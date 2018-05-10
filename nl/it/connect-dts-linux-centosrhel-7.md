---

copyright:
  years: 2017
lastupdated: "2017-11-13"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Connessione al dispositivo DTS in Linux per CentOS/RHEL 7

Per interagire con una LUN iSCSI nei sistemi operativi basati su Linux, gli utenti devono stabilire una connessione alla LUN immettendo una serie di comandi nel terminale sulla base del sistema operativo utilizzato per eseguire le interazioni. Lo strumento utilizzato per interagire con una LUN iSCSI in un sistema operativo basato su Linux dipende dal tipo e della versione del sistema operativo installato sul dispositivo.

## Istruzioni per CentOS 7 e RHEL 7

1. Installa iscsi-initiator e il mapper a percorsi multipli per Linux <br/>
   ``yum -y install iscsi-initiator-utils device-mapper device-mapper-multipath`` 
2. Crea il file di configurazione iscsid.conf <br/>
3. Esegui un backup della configurazione originale: <br/>
   ``cp /etc/iscsi/iscsid.conf{,.save}`` 
4. Apri /etc/iscsi/iscsid.conf con il tuo editor di testo preferito e sostituisci il contenuto con quanto segue: <br/>
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
5. Avvia iscsid:<br/>
   ``/etc/init.d/iscsi start``
6. Esegui un rilevamento sull'host di destinazione iscsi:<br/>
   ``iscsiadm -m discovery -t sendtargets -p [indirizzo IP in StorageLayer]``
7. Stabilisci una connessione all'host di destinazione iscsi:<br/>
   ``iscsiadm -m node -T [output from above starting with iqn.] -p [indirizzo IP in storagelayer] -l``
8. Riavvia il servizio iscsi (poiché node.startup era impostato su automatic in iscsid.conf, eseguirà automaticamente l'accesso all'host di destinazione).<br/>
   ``/etc/init.d/iscsi restart``
