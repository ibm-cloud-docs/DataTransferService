---

copyright:
  years: 2017, 2019
lastupdated: "2019-02-05"

---
{:new_window: target="_blank"}

# Einführung in den Data Transfer-Service
{: #gettingstarted}

Mit dem Data Transfer Service von {{site.data.keyword.BluSoftlayer_full}} können Kunden eine mit USB 2.0 oder USB 3.0 kompatible Einheit, CDs und DVDs an ein {{site.data.keyword.BluSoftlayer}}-Rechenzentrum senden. Die Einheit wird direkt mit dem Netz des Kunden verbunden, sodass dieser die Datenübertragung über Fernzugriff steuern kann. Die Einheit befindet sich in einem dedizierten Rack im Rechenzentrum des Kunden und wird als iSCSI-Ziel angehängt. Der Data Transfer-Service ist ideal für die Übertragung großer Datenvolumen unabhängig vom privaten Netz von {{site.data.keyword.BluSoftlayer}}. Dieser Service steht allen {{site.data.keyword.BluSoftlayer}}-Kunden kostenlos zur Verfügung.

## Anzeige des Data Transfer-Service aufrufen

**Hinweis**: Diese Anzeige ist nur für den Masterbenutzer des Kontos verfügbar.

1. Verwenden Sie die eindeutigen Berechtigungsnachweise, um auf das [{{site.data.keyword.slportal}} ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/){:new_window} zuzugreifen. 
2. Wählen Sie in der Navigationsleiste **Speicher** > **Datenmigration** > **Data Transfer** aus, um die Anzeige für den Data Transfer-Service zu öffnen. <br/>

In der Anzeige **Data Transfer Service** können Benutzer eine Datenübertagungsanforderung abschicken, Details zu einer Anforderung anzeigen, das Ticketprotokoll zur Einheitenüberwachung anzeigen sowie eine vorhandene Anforderung abbrechen.

## Data Transfer-Anforderung übergeben

Durch Data Transfer-Anforderungen werden die zuständigen Personen in unseren Rechenzentren davon in Kenntnis gesetzt, dass eine Lieferung von einem Kunden zu erwarten ist. Anforderungen werden über das [{{site.data.keyword.slportal}} ![Symbol für externen Linnk](../../icons/launch-glyph.svg "Symbol für externen Linnk")](https://control.softlayer.com/){:new_window} übergeben. 

Beachten Sie beim Erstellen einer Anforderung die folgenden Richtlinien.

- Stellen Sie sicher, dass die Einheit, die Sie einsenden möchten, alle [Hardwarevoraussetzungen](/docs/infrastructure/DataTransferService/data-transfer-service-faq.html) erfüllt.
- Jeder Anforderung kann nur eine einzelne Einheit zugeordnet werden. Wenn Sie mehrere Einheiten einsenden möchten, erstellen Sie für jede Einheit eine neue Anforderung.
- Wenn die Einheit zurückgesandt werden soll, legen Sie Ihrer Sendung freigemachte Versandaufkleber sowie gegebenenfalls die erforderlichen Exportdokumente bei, damit die Einheit nach Ablauf des Übertragungszeitraums zurückgesendet werden kann.
- Beim Versand ins Ausland sind Sie für die Lizenzierung, den Transport und die Zollabfertigung für die Einheit verantwortlich. Dies umfasst auch die Bezahlung aller Gebühren, Steuern und Versandkosten zum und vom (falls zutreffend) {{site.data.keyword.BluSoftlayer}}-Rechenzentrum.
- Beim Abschließen der Anforderung müssen Sie den Namen und die Tracking-Nummer des beauftragten Transportunternehmens angeben.  Erstellen Sie den Versandaufkleber mit der Adresse des entsprechenden Rechenzentrums, bevor Sie die Data Transfer-Anforderung übergeben.

Führen Sie diese Schritte aus, um eine Data Transfer-Anforderung zu übergeben. 

1. Öffnen Sie die Anzeige des **Data Transfer Service** im [{{site.data.keyword.slportal}} ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/){:new_window}. 
2. Klicken Sie auf **Data Transfer-Anforderung bestellen**.
3. Füllen Sie die Felder im Abschnitt **Einheitendaten** gemäß Tabelle 1 aus.
<table border="1">
<caption>In Tabelle 1 sind die Namen der Felder des Anforderungsformulars links und die zugehörigen Beschreibungen rechts aufgeführt.</caption>
 <tr><th>Feldname</th><th>Anweisungen</th></tr>
 <tr><td>Einheitentyp</td><td>Der Typ der Einheit, die an den Bestimmungsort gesendet wird. Wenn der Einheitentyp nicht in der Liste aufgeführt ist, wählen Sie "Andere" aus.</td></tr>
 <tr><td>Seriennummer</td><td> Die Seriennummer der Einheit.</td></tr><tr><td>Beschreibung</td><td>Eine kurze Beschreibung der Einheit. Wichtige Details sind eindeutige Merkmale wie zum Beispiel Farbe, Beschriftungen oder Aufkleber usw.</td></tr>
 <tr><td>Hinweis</td><td>Zusätzliche Angaben zum Gerät oder zur Übertragung.</td></tr><tr><td>Ziel</td><td>Das Rechenzentrum, an das das Gerät gesendet werden soll.</td></tr>
 <tr><td>Zusteller</td><td>Der Post- oder Expresszusteller, der die Einheit zum Zielort transportiert.</td></tr>
 <tr><td>Tracking-Nummer</td><td>Die vollständige Tracking-Nummer für die Sendungsverfolgung.</td></tr>
 </table>

4. Füllen Sie alle Felder im Abschnitt **Rücksendeadresse** aus oder wählen Sie **Firmenadresse** aus, damit die gespeicherte Firmenadresse automatisch in die Felder eingetragen wird. <br/> **Hinweis**: Legen Sie Ihrer Sendung freigemachte Rücksendeaufkleber sowie gegebenenfalls erforderliche Exportdokumente bei.
5. Lesen Sie die bereitgestellten Servicevereinbarungen und wählen Sie anschließend das Kontrollkästchen **Ich habe die Vereinbarung für den Data Transfer-Service und die Rahmenvereinbarung gelesen und stimme ihnen zu** aus.
6. Klicken Sie auf **Serviceanforderung abschicken**.

Nach dem Abschicken der Anforderung wird für das Anforderungsticket der Status `An SoftLayer gesendet` angezeigt. Bitte informieren Sie {{site.data.keyword.BluSoftlayer}}, wenn für eine Import- oder Exportsendung eine Lizenz Ihrer lokalen Behörden erforderlich ist, und geben Sie die Lizenzinformationen im Ticket an.

Nachdem die Einheit zugestellt ist, wird der Status in *Von SoftLayer empfangen* aktualisiert. Der Ticketstatus wird später in *Verbunden* aktualisiert, nachdem ein Techniker des Rechenzentrums die Einheit mit dem Netz verbunden hat.

Der erste Data Transfer-Zeitraum umfasst zwei Wochen. In diesem Zeitraum kann allein der Kontoadministrator auf die Einheit zugreifen. Wenn Sie mehr Zeit benötigen, können Sie eine Verlängerung anfordern. Falls die Einheit bereits vor Ablauf der zwei Wochen zurückgesendet werden soll, kann eine entsprechende Rücksendeanforderung erstellt werden. Sie müssen {{site.data.keyword.IBM}} über das [{{site.data.keyword.slportal}}](https://control.softlayer.com/) informieren, sobald die Übertragung abgeschlossen ist. Daraufhin wird die Einheit von {{site.data.keyword.BluSoftlayer}} entfernt und gemäß Ihrer Anforderung entweder zurückgeschickt oder vernichtet.


## Versandanzeige aufrufen

In der Versandanzeige im [{{site.data.keyword.slportal}} ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/){:new_window} werden alle Versandvorgänge im Zusammenhang mit Anforderungen für den Data Transfer-Service angezeigt. In dieser Anzeige können Sendungen angezeigt und Rücksendungen nach Erhalt bestätigt werden.

Gehen Sie wie folgt vor, um auf die Versandanzeige zuzugreifen:

1. Verwenden Sie die eindeutigen Berechtigungsnachweise, um auf das [{{site.data.keyword.slportal}} ![Symbol für externen Link](../../icons/launch-glyph.svg "Symbol für externen Link")](https://control.softlayer.com/){:new_window} zuzugreifen. 
2. Wählen Sie in der Navigationsleiste **Konto** > **Verwalten** > **Versand** aus.

In der Versandanzeige werden alle Versandanforderungen der letzten 30 Tage zusammen mit den zugehörigen Details angezeigt. Die Lieferungen können nach Status, Alter oder nach bestimmten Lieferdetails [sortiert oder gefiltert](sort-or-filter-shipments-list.html) werden. Außerdem kann in dieser Anzeige der Empfang von Rücksendungen bestätigt werden.
![Anzeige 'Versand'](/images/DTSShipmentScreen1.png)
