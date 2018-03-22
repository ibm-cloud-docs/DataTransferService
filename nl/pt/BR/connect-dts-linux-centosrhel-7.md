---

copyright:
  years: 2017
lastupdated: "2017-11-13"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Conectando-se ao dispositivo DTS no Linux for CentOS/RHEL 7

Para interagir com uma LUN iSCSI em sistemas operacionais baseados em Linux, os usuários devem se conectar à LUN inserindo uma série de comandos no terminal com base no sistema operacional que está sendo usado para executar as interações. A ferramenta usada para interagir com uma LUN iSCSI em um OS baseado no Linux é dependente do tipo e versão do OS instalado no dispositivo.

## Instruções para o CentOS 7 e o RHEL 7

1. Instale o inicializador iSCSI e o mapeador de caminhos múltiplos para Linux <br/>
   ``yum -y install iscsi-initiator-utils device-mapper device-mapper-multipath`` 
2. Crie o arquivo de configuração iscsid.conf <br/>
3. Faça backup da configuração original: <br/>
   ``cp /etc/iscsi/iscsid.conf{,.save}`` 
4. Abra /etc/iscsi/iscsid.conf com seu editor de texto favorito e substitua o conteúdo pelo seguinte: <br/>
   ``node.startup = automatic ``<br/>
   ``node.session.auth.username = ISCSI_USER ``<br/>
   ``node.session.auth.password = ISCSI_PASS ``<br/>
   ``discovery.sendtargets.auth.username = ISCSI_USER ``<br/>
   ``discovery.sendtargets.auth.password = ISCSI_PASS ``<br/>
   ``node.session.timeo.replacement_timeout = 120 ``<br/>
   ``node.conn[0].timeo.login_timeout = 15 ``<br/>
   ``node.conn[0].timeo.logout_timeout = 15 ``<br/>
   ``node.conn[0].timeo.noop_out_interval = 10 ``<br/>
   ``node.conn[0].timeo.noop_out_timeout = 15 ``<br/>
   ``node.session.iscsi.InitialR2T = No ``<br/>
   ``node.session.iscsi.ImmediateData = Yes ``<br/>
   ``node.session.iscsi.FirstBurstLength = 262144 ``<br/>
   ``node.session.iscsi.MaxBurstLength = 16776192 ``<br/>
   ``node.conn[0].iscsi.MaxRecvDataSegmentLength = 65536 ``<br/>
5. Inicie iscsid:<br/>
   ``/etc/init.d/iscsi start``
6. Execute uma descoberta no host de destino iscsi:<br/>
   ``iscsiadm -m discovery -t sendtargets -p [IP Address in StorageLayer]``
7. Conecte-se ao host de destino iscsi:<br/>
   ``iscsiadm -m node -T [output from above starting with iqn.] -p [IP Address in storagelayer] -l``
8. Reinicie o serviço iscsi (como o node.startup foi configurado para automatic no iscsid.conf, ele efetuará login automaticamente no host de destino).<br/>
   ``/etc/init.d/iscsi restart``
