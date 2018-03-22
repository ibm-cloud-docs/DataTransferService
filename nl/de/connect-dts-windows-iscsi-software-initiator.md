---

copyright:
  years: 2017
lastupdated: "2017-11-13"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Verbindung zu DTS-Einheit unter Windows mit iSCSI Software Initiator herstellen

Für die Interaktion mit einem iSCSI-LUN unter Windows muss die Verbindung zum LUN mit iSCSI Software Initiator, dem proprietären iSCSI-Tool von Microsoft, hergestellt werden. Bei Verwendung von Windows Server 2008 oder Windows Vista und höheren Windows-Versionen ist iSCSI Software Initiator in das Betriebssystem integriert. Für Windows Server 2003, Windows XP und Windows 2000 muss die Initiator-Software heruntergeladen werden, bevor diese Prozedur ausgeführt wird. Führen Sie die folgenden Schritte aus, um unter Windows mit iSCSI Software Initiator die Verbindung zu einem iSCSI-LUN herzustellen.

## Verbindung zu einem iSCSI-LUN herstellen

1. Rufen Sie **iSCSI-Benutzername, Kennwort und Speicheradresse** für die iSCSI-Instanz, die verbunden werden soll, im Kundenportal ab. Weitere Informationen finden Sie im Abschnitt zum Aufrufen der Anzeige für Datenübertragung.
2. Starten Sie den iSCSI-Initiator.
3. Geben Sie als Initiatornamen auf der Registerkarte **Konfiguration** die IQN-Daten aus dem SoftLayer-Portal an.
4. Klicken Sie auf die Registerkarte **Erkennung**b.
5. Klicken Sie auf die Schaltfläche **Hinzufügen** im Abschnitt **Zielportale** der Anzeige.
6. Geben Sie die **iSCSI-IP-Adresse** in das Feld **IP-Adresse oder DNS-Name** ein.
7. Klicken Sie auf die Registerkarte **Erweitert**.
8. Aktualisieren Sie die Anmeldedaten für iSCSI.
   - Wählen Sie das Kontrollkästchen **CHAP-Anmeldedaten** aus, um die CHAP-Anmeldung zu aktivieren.
   - Geben Sie den **iSCSI-Benutzernamen** in das Feld **Benutzername** ein.
   - Geben Sie das **iSCSI-Kennwort** in das Feld **Geheimer Schlüssel für Ziel** ein.
   - Klicken Sie zweimal auf die Schaltfläche **OK**.
9. Klicken Sie auf die Registerkarte **Ziele**.
10. Wählen Sie den neu hinzugefügten iSCSI-Eintrag in der Liste **Ziele** aus.
11. Klicken Sie auf die Schaltfläche **Anmelden**. Das Popup-Menü **Beim Ziel anmelden** wird angezeigt.
12. Wählen Sie das Kontrollkästchen **Verbindung bei Systemstart automatisch wiederherstellen** aus, damit die Verbindung auch nach einem Warmstart erhalten bleibt.
13. Klicken Sie auf die Schaltfläche **Erweitert**.
14. Aktualisieren Sie die Anmeldedaten für iSCSI.
    - Wählen Sie das Kontrollkästchen **CHAP-Anmeldedaten** aus, um die CHAP-Anmeldung zu aktivieren.
    - Geben Sie den **iSCSI-Benutzernamen** in das Feld **Benutzername** ein.
    - Geben Sie das **iSCSI-Kennwort** in das Feld **Geheimer Schlüssel für Ziel** ein.
    - Klicken Sie zweimal auf die Schaltfläche **OK**.
15. Überprüfen Sie, ob das neue iSCSI-Ziel auf der Registerkarte 'Ziele' als 'Verbunden' angezeigt wird.

<table>
<tbody>
<tr>
<th>iSCSI-Ziel</th><th>Folgendes ausführen</th></tr>
<tr><td>Wird als 'Verbunden' angezeigt</td><td>Klicken Sie auf die Schaltfläche <strong>OK</strong>. Ihre iSCSI-LUN ist jetzt verbunden.</td></tr>
<tr><td>Wird nicht als 'Verbunden' angezeigt</td><td>Wiederholen Sie die oben angegebenen Schritte, um die Verbindung zurückzusetzen.</td></tr></tbody></table>
