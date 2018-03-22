---

copyright:
  years: 2017
lastupdated: "2017-11-13"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Verbindung zu DTS-Einheit unter Linux for CentOS/RHEL 7 herstellen

Für die Interaktion mit einem iSCSI-LUN unter Linux-basierten Betriebssystemen müssen Sie die Verbindung zum LUN herstellen, indem Sie eine Reihe von Befehlen in einem Terminal für das jeweilige Betriebssystem absetzen. Welches Tool für die Interaktion mit einem iSCSI-LUN unter einem Linux-basierten Betriebssystem verwendet wird, hängt vom Typ und von der Version des in der betreffenden Einheit installierten Betriebssystems ab.

## Anweisungen für CentOS 7 und RHEL 7

1. Installieren Sie den iSCSI-Initiator und den Multipath-Mapper für Linux <br/>
   ``yum -y install iscsi-initiator-utils device-mapper device-mapper-multipath`` 
2. Erstellen Sie die Konfigurationsdatei iscsid.conf <br/>
3. Sichern Sie die ursprüngliche Konfiguration: <br/>
   ``cp /etc/iscsi/iscsid.conf{,.save}`` 
4. Öffnen Sie die Datei /etc/iscsi/iscsid.conf mit Ihrem bevorzugten Texteditor und ersetzen Sie den Inhalt durch die folgenden Angeben: <br/>
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
5. Starten Sie iSCSI:<br/>
   ``/etc/init.d/iscsi start``
6. Führen Sie eine Erkennung für den iSCSI-Zielhost durch:<br/>
   ``iscsiadm -m discovery -t sendtargets -p [IP-Adresse in StorageLayer]``
7. Stellen Sie eine Verbindung zum iSCSI-Zielhost her:<br/>
   ``iscsiadm -m node -T [Ausgabe des Vorhergehenden, beginnend mit iqn.] -p [IP-Adresse in StorageLayer] -l``
8. Starten Sie den iSCSI-Service erneut (da für node.startup in iscsid.conf die automatische Ausführung festgelegt wurde, erfolgt die Anmeldung beim Zielhost automatisch).<br/>
   ``/etc/init.d/iscsi restart``
