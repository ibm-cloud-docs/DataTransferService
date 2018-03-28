---

copyright:
  years: 2017
lastupdated: "2017-11-13"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Conexión al dispositivo DTS en Linux for CentOS/RHEL 7

Para interactuar con un LUN iSCSI en sistemas operativos basados en Linux, los usuarios deben conectar el LUN especificando una serie de mandatos en el terminal basados en el sistema operativo utilizado para realizar las interacciones.  La herramienta utilizada para interactuar con un LUN iSCSI en un sistema operativo Linux depende del tipo y de la versión del sistema operativo instalado en el dispositivo.

## Instrucciones para CentOS 7 y RHEL 7

1. Instale iscsi-initiator y un correlacionador multivía de acceso para Linux <br/>
   ``yum -y install iscsi-initiator-utils device-mapper device-mapper-multipath`` 
2. Cree el archivo de configuración iscsid.conf <br/>
3. Realice una copia de seguridad de la configuración original: <br/>
   ``cp /etc/iscsi/iscsid.conf{,.save}`` 
4. Abra /etc/iscsi/iscsid.conf con el editor de texto que prefiera y sustituya el contenido con lo siguiente: <br/>
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
6. Ejecute un descubrimiento sobre el host de destino de iscsi:<br/>
   ``iscsiadm -m discovery -t sendtargets -p [IP Address in StorageLayer]``
7. Conéctese al host de destino de iscsi:<br/>
   ``iscsiadm -m node -T [output from above starting with iqn.] -p [IP Address in storagelayer] -l``
8. Reinicie el servicio iscsi (como node.startup se ha establecido en automatic en iscsid.conf, iniciará automáticamente una sesión en el host de destino).<br/>
   ``/etc/init.d/iscsi restart``
