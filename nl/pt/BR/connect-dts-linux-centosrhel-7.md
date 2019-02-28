---

copyright:
  years: 2017, 2019
lastupdated: "2019-02-05"

---
{:pre: .pre}

# Conectando-se ao dispositivo DTS no Linux for CentOS/RHEL 7
{: #mountingDTSlinux}

Para interagir com uma LUN iSCSI em sistemas operacionais baseados em Linux, os usuários devem se conectar ao LUN inserindo uma série de comandos no terminal. A ferramenta usada para interagir com uma LUN iSCSI em um S.O. baseado no Linux depende do tipo e da versão do S.O. instalado no dispositivo.

## Configurando a conexão no CentOS 7 e no RHEL 7

1. Instale o inicializador iSCSI e os utilitários do mapeador de caminhos múltiplos para o Linux.
   ```
   yum -y install iscsi-initiator-utils device-mapper device-mapper-multipath
   ```
   {: pre}

2. Crie o arquivo de configuração  ` iscsid.conf ` .

3. Faça backup da configuração original.
   ```
   cp /etc/iscsi/iscsid.conf{,.save}
   ```
   {: pre}

4. Abra `/etc/iscsi/iscsid.conf` com o seu editor de texto favorito e substitua o conteúdo pelo código a seguir:
   ```
   node.startup = automatic
   node.session.auth.username = ISCSI_USER
   node.session.auth.password = ISCSI_PASS
   discovery.sendtargets.auth.username = ISCSI_USER
   discovery.sendtargets.auth.password = ISCSI_PASS
   node.session.timeo.replacement_timeout = 120
   node.conn[0].timeo.login_timeout = 15
   node.conn[0].timeo.logout_timeout = 15
   node.conn[0].timeo.noop_out_interval = 10
   node.conn[0].timeo.noop_out_timeout = 15
   node.session.iscsi.InitialR2T = No
   node.session.iscsi.ImmediateData = Yes
   node.session.iscsi.FirstBurstLength = 262144
   node.session.iscsi.MaxBurstLength = 16776192
   node.conn[0].iscsi.MaxRecvDataSegmentLength = 65536
   ```
   {: pre}

5. Inicie o iSCSI.<br/>
   ```
   systemctl start iscsi.service
   ```
   {: pre}

6. Execute uma descoberta com relação ao host de destino iscsi.<br/>
   ```
   iscsiadm -m discovery -t sendtargets -p [IP address in StorageLayer]
   ```
   {: pre}

7. Conecte-se ao host de destino iscsi.<br/>
   ```
   iscsiadm -m node -T [output from previous command, starting with IQN.] -p [IP address in StorageLayer] -l
   ```
   {: pre}

8. Reinicie o serviço iSCSI. Como o `node.startup` está configurado como automático em `iscsid.conf`, ele efetua login automaticamente no host de destino.<br/>
   ```
   systemctl restart iscsi.service
   ```
   {: pre}
