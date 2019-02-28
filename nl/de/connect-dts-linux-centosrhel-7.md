---

copyright:
  years: 2017, 2019
lastupdated: "2019-02-05"

---
{:pre: .pre}

# Verbindung zu DTS-Einheit unter Linux for CentOS/RHEL 7 herstellen
{: #mountingDTSlinux}

Für die Interaktion mit einem iSCSI-LUN unter Linux-basierten Betriebssystemen müssen Sie die Verbindung zum LUN herstellen, indem Sie eine Reihe von Befehlen in einem Terminal absetzen. Welches Tool für die Interaktion mit einem iSCSI-LUN unter einem Linux-basierten Betriebssystem verwendet wird, hängt vom Typ und von der Version des in der betreffenden Einheit installierten Betriebssystems ab.

## Verbindung in CentOS 7 und RHEL 7 konfigurieren

1. Installieren Sie die Dienstprogramme iSCSI Initiator und Multipath Mapper für Linux.
   ```
   yum -y install iscsi-initiator-utils device-mapper device-mapper-multipath
   ```
   {: pre}

2. Erstellen Sie die Konfigurationsdatei `iscsid.conf`.

3. Erstellen Sie einer Sicherungskopie der ursprünglichen Konfiguration.
   ```
   cp /etc/iscsi/iscsid.conf{,.save}
   ```
   {: pre}

4. Öffnen Sie die Datei `/etc/iscsi/iscsid.conf` mit dem bevorzugten Texteditor und ersetzen Sie den Inhalt durch den folgenden Code:
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

5. Starten Sie iSCSI.<br/>
   ```
   systemctl start iscsi.service
   ```
   {: pre}

6. Führen Sie eine Erkennung für den iSCSI-Zielhost durch.<br/>
   ```
   iscsiadm -m discovery -t sendtargets -p [IP address in StorageLayer]
   ```
   {: pre}

7. Stellen Sie eine Verbindung zum iSCSI-Zielhost her.<br/>
   ```
   iscsiadm -m node -T [Ausgabe des vorherigen Befehls, beginnend mit IQN.] -p [IP address in StorageLayer] -l
   ```
   {: pre}

8. Starten Sie den iSCSI-Service erneut. Da für `node.startup` in `iscsid.conf` die automatische Ausführung festgelegt ist, erfolgt die Anmeldung beim Zielhost automatisch.<br/>
   ```
   systemctl restart iscsi.service
   ```
   {: pre}
