---

copyright:
  years: 2017, 2019
lastupdated: "2019-02-05"

---
{:pre: .pre}

# Connessione al dispositivo DTS in Linux per CentOS/RHEL 7
{: #mountingDTSlinux}

Per interagire con una LUN iSCSI in sistemi operativi basati su Linux, gli utenti devono stabilire una connessione alla LUN immettendo una serie di comandi nel terminale. Lo strumento utilizzato per interagire con una LUN iSCSI in un sistema operativo basato su Linux dipende dal tipo e della versione del sistema operativo installato sul dispositivo.

## Configurazione della connessione in CentOS 7 e RHEL 7

1. Installa l'iniziatore iSCSI e il programma di utilità del mapper a percorsi multipli per Linux.
   ```
   yum -y install iscsi-initiator-utils device-mapper device-mapper-multipath
   ```
   {: pre}

2. Crea il file di configurazione `iscsid.conf`.

3. Esegui il backup della configurazione originale.
   ```
   cp /etc/iscsi/iscsid.conf{,.save}
   ```
   {: pre}

4. Apri `/etc/iscsi/iscsid.conf` con il tuo editor di testo preferito e sostituisci il contenuto con il seguente codice:
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

5. Avvia iSCSI.<br/>
   ```
   systemctl start iscsi.service
   ```
   {: pre}

6. Esegui un rilevamento sull'host di destinazione iscsi.<br/>
   ```
   iscsiadm -m discovery -t sendtargets -p [indirizzo IP in StorageLayer]
   ```
   {: pre}

7. Stabilisci una connessione all'host di destinazione iscsi.<br/>
   ```
   iscsiadm -m node -T [output dal comando precedente, iniziando con IQN.] -p [indirizzo IP in StorageLayer] -l
   ```
   {: pre}

8. Riavvia il servizio iSCSI. Poiché `node.startup` è impostato su automatic in `iscsid.conf` esegue automaticamente l'accesso all'host di destinazione.<br/>
   ```
   systemctl restart iscsi.service
   ```
   {: pre}
