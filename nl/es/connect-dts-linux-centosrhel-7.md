---

copyright:
  years: 2017, 2018
lastupdated: "2017-05-22"

---
{:pre: .pre}

# Conexión al dispositivo DTS en Linux for CentOS/RHEL 7

Para interactuar con un LUN iSCSI en sistemas operativos basados en Linux, los usuarios deben conectar el LUN especificando una serie de mandatos en el terminal. La herramienta utilizada para interactuar con un LUN iSCSI en un sistema operativo Linux depende del tipo y de la versión del sistema operativo instalado en el dispositivo.

## Instrucciones para CentOS 7 y RHEL 7

1. Instale iscsi-initiator y un correlacionador multivía de acceso para Linux.
   ```
   yum -y install iscsi-initiator-utils device-mapper device-mapper-multipath
   ``` 
   {: pre}
   
2. Cree el archivo de configuración iscsid.conf.

3. Realice una copia de seguridad de la configuración original:
   ```
   cp /etc/iscsi/iscsid.conf{,.save}
   ``` 
   {: pre}
   
4. Abra /etc/iscsi/iscsid.conf con el editor de texto que prefiera y sustituya el contenido con el código siguiente: 
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

5. Inicie iscsi:<br/>
   ```
   /etc/init.d/iscsi start
   ```
   {: pre}
   
6. Ejecute un descubrimiento sobre el host de destino de iscsi:<br/>
   ```
   iscsiadm -m discovery -t sendtargets -p [IP address in StorageLayer]
   ```
   {: pre}
   
7. Conéctese al host de destino de iscsi:<br/>
   ```
   iscsiadm -m node -T [output from previous command, starting with IQN.] -p [IP address in StorageLayer] -l
   ```
   {: pre}
   
8. Reinicie el servicio iscsi (como node.startup se ha establecido en automático en iscsid.conf, iniciará automáticamente una sesión en el host de destino).<br/>
   ```
   /etc/init.d/iscsi restart
   ```
   {: pre}
