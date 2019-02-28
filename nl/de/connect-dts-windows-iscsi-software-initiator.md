---

copyright:
  years: 2017, 2019
lastupdated: "2019-02-05"

---


# Verbindung zu DTS-Einheit unter Windows mit iSCSI Software Initiator herstellen
{: #mountingDTSWindows}

Für die Interaktion mit einem iSCSI-LUN unter Windows muss die Verbindung zum Speicher mit iSCSI Software Initiator, dem proprietären iSCSI-Tool von Microsoft, hergestellt werden. Bei Verwendung von Windows Server 2008 oder Windows Vista und höheren Windows-Versionen ist iSCSI Software Initiator in das Betriebssystem integriert. Für Windows Server 2003, Windows XP und Windows 2000 muss die Initiator-Software heruntergeladen werden, bevor diese Prozedur ausgeführt wird.

## Verbindung zu einem iSCSI-LUN herstellen

1. Rufen Sie vom {{site.data.keyword.slportal}} den **iSCSI-Benutzernamen, das Kennwort und die Speicheradresse** für die Speichereinheit ab, für die eine Verbindung hergestellt werden soll.
2. Starten Sie iSCSI Initiator.
3. Aktualisieren Sie auf der Registerkarte **Konfiguration** den Initiatornamen, indem Sie die IQN-Daten im {{site.data.keyword.slportal}} angeben.
4. Klicken Sie auf **Erkennung**.
5. Klicken Sie im Abschnitt **Zielportale** auf **Hinzufügen**.
6. Geben Sie im Feld **IP-Adresse oder DNS-Name** die **iSCSI-IP-Adresse** ein.
7. Klicken Sie auf **Erweitert**.
8. Aktualisieren Sie die Anmeldedaten für iSCSI.
   - Wählen Sie das Kontrollkästchen **CHAP-Anmeldedaten** aus, um die CHAP-Anmeldung zu aktivieren.
   - Geben Sie den iSCSI-Benutzernamen im Feld **Benutzername** ein.
   - Geben Sie das iSCSI-Kennwort im Feld **Geheimer Schlüssel für Ziel** ein.
   - Klicken Sie zweimal auf **OK**.
9. Klicken Sie auf **Ziele**
10. Wählen Sie den neu hinzugefügten iSCSI-Eintrag in der Liste **Ziele** aus.
11. Klicken Sie auf **Anmelden**. Das Fenster **Beim Ziel anmelden** wird angezeigt.
12. Wählen Sie **Verbindung bei Systemstart automatisch wiederherstellen** aus, damit die Verbindung auch nach einem Neustart erhalten bleibt.
13. Klicken Sie auf **Erweitert**.
14. Aktualisieren Sie die Anmeldedaten für iSCSI.
    - Wählen Sie das Kontrollkästchen **CHAP-Anmeldedaten** aus, um die CHAP-Anmeldung zu aktivieren.
    - Geben Sie den iSCSI-Benutzernamen im Feld **Benutzername** ein.
    - Geben Sie das iSCSI-Kennwort im Feld **Geheimer Schlüssel für Ziel** ein.
    - Klicken Sie zweimal auf **OK**.
15. Überprüfen Sie, ob das neue iSCSI-Ziel auf der Registerkarte 'Ziele' als 'Verbunden' angezeigt wird.
    - Wenn für das iSCSI-Ziel **Verbunden** angezeigt wird, klicken Sie auf **OK**. Ihre iSCSI-LUN ist jetzt verbunden.
    - Wenn für das iSCSI-Ziel nicht **Verbunden** angezeigt wird, wiederholen Sie die vorherigen Schritte, um die Verbindung zurückzusetzen.
