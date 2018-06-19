---

copyright:
  years: 1994, 2018
lastupdated: "2018-05-22"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Häufig gestellte Fragen

## Was ist Data Transfer?

Mit diesem Service können berechtigte Benutzer (in der Regel der Kontoadministrator) kompatible Einheiten an eines unserer Rechenzentren senden, damit sie direkt mit dem Kontonetz verbunden werden. Die Einheit befindet sich in einem dedizierten Rack und ist für einen Zeitraum von zwei Wochen als iSCSI-Ziel angehängt. In diesem Zeitraum kann der Administrator die Einheit im Netz aufrufen und zusammen mit anderen Einheiten und Services in dem zugehörigen Konto nutzen. Nach Ablauf der zwei Wochen kann eine Verlängerung angefordert werden, damit die Einheit weiterhin mit dem Netz verbunden bleibt. Andernfalls wird die Einheit entweder an die Partei zurückgegeben, die beim Erstellen der Anforderung angegeben wurde, oder die Einheit wird vor Ort vernichtet. 

## Kann ich eine Einheit für Data Transfer international versenden?

Hardware und Datenträger können an jedes unserer Rechenzentren im In- und Ausland versendet werden. Dabei sind Sie als Kunde für Folgendes verantwortlich: 

- Sicherstellen, dass für den Versand der Einheit an das {{site.data.keyword.IBM}} Rechenzentrum oder für die Rücksendung zum Kunden (falls zutreffend) keine Import- oder Exportgenehmigung erforderlich ist.
- Sicherstellen, dass weder für den Kunden noch für etwaige Benutzer des Kunden, deren Daten im Inhalt enthalten sind, gesetzliche Bestimmungen in den USA gelten, die ihre bestehenden Exportberechtigungen in den USA aussetzen oder widerrufen. Sie müssen {{site.data.keyword.IBM}} unverzüglich informieren, wenn Ihr Unternehmen oder ein beteiligter Benutzer einer solchen gesetzlichen Bestimmung unterliegt.
- Lizenzierung, Transport und Zollabfertigung für die Einheit, einschließlich aller Gebühren, Steuern und Versandkosten zum und vom {{site.data.keyword.IBM}} Rechenzentrum (falls zutreffend).
- Einhaltung aller anwendbaren Gesetze, einschließlich Datenschutz-, Import- und Exportgesetze, im Zusammenhang mit der Zustellung und Rücksendung der Einheit sowie der Übertragung von Inhalten zum {{site.data.keyword.IBM}} Rechenzentrum.
- Abschließen geeigneter Vereinbarungen und Einholen erforderlicher Genehmigungen beim Benutzer des Kunden für alle Benutzerdaten, die der Kunde in die Hardware übertragen wird.

Legen Sie Ihrer Sendung ein freigemachtes Rücksendeetikett sowie alle zugehörigen Exportdokumente bei, damit wir die Einheit ordnungsgemäß verpacken, dokumentieren und adressieren können. Wenn keine Rücksendung angefordert wird, wird die Einheit vernichtet.


## Welche Einheitentypen kann ich mit einer Data Transfer-Anforderung senden?
Halten Sie beim Auswählen einer Einheit oder eines Datenträgers (CD oder DVD) zum Einsenden für Data Transfer die folgenden Richtlinien ein:

- Hardwarevoraussetzungen:
   - Die Stromversorgung muss mit einer Spannung von 208 V bzw. 220 V kompatibel sein.

   - Der Netzstecker muss in eine 120 V-Steckdose (NEMA 5-15P) passen.

   - Die Einheit muss mit USB 2.0 oder USB 3.0 kompatibel sein.

   - Ein USB-Stecker (USB-Standardstecker, geeignet für die meisten Computer) muss vorhanden sein.

- Voraussetzungen für CD/DVD:

   - Datenträger müssen in CD-Alben, Transportbehältern oder ähnlichen Schutzhüllen eingesandt werden. Verpacken Sie mehrere Datenträger zum Einsenden in einem einzigen Behälter oder CD-Album.

   - Jeder Datenträger muss gut lesbar und eindeutig beschriftet sein (z. B. Datenträger A, Datenträger B, Datenträger C usw.).

## Kann meine Einheit schon vor der zweiwöchigen Frist zurückgesendet oder länger als zwei Wochen aufbewahrt werden?

Ja, Ihre Hardware oder Datenträger können bei Bedarf an einem beliebigen Zeitpunkt zurückgesandt werden oder über den üblichen Zeitraum hinaus verbunden bleiben. Um eine frühere Rückgabe oder längere Bereitstellung anzufordern, fügen Sie im ursprünglichen Ticket der Data Transfer-Anforderung einen entsprechenden Kommentar hinzu. Wenn die Rücksendung gewünscht ist, entnehmen wir die Hardware bzw. die Datenträger aus dem System und senden Sie unter Verwendung der von Ihnen bereitgestellten Verpackung und der freigemachten Versandaufkleber an die Rücksendeadresse, die in der ursprünglichen Anforderung angegeben wurde.

Jede Verlängerungsanforderung wird schnellstmöglich verarbeitet. Dabei ist zu beachten, dass jede Verlängerungsanforderung die Verbindungszeit der Einheit um eine Woche verlängert. Für den Verlängerungszeitraum werden gegebenenfalls zusätzliche Gebühren berechnet. Weitere Details werden bereitgestellt, wenn ein Mitglied unseres Teams auf die Anforderung in dem ursprünglichen Ticket antwortet.

## Was bedeuten die verschiedenen Statusangaben in meinem Data Transfer-Ticket?

Jeder Status im Data Transfer-Ticket gibt die Phase des Übertragungsprozesses für die Hardware bzw. die Datenträger an, die an das Rechenzentrum eingesandt wurden. Weitere Details zu den einzelnen Status enthält die nachfolgende Tabelle:

|Status 	| Definition |
|---------| -----------|
|An SoftLayer gesendet 	|Die Data Transfer-Anforderung wurde vom Benutzer abgeschickt und die Hardware bzw. Datenträger werden an das ausgewählte Rechenzentrum ausgeliefert.|
|Von SoftLayer empfangen |	Die Sendung wurde im Rechenzentrum empfangen, die Einheit wurde unter einer Seriennummer registriert und in unser System eingelesen.|
|Verbunden |	Die Hardware bzw. der Datenträger ist mit der Einheit verbunden.|
|Bereitgestellt |	Für die Einheit wird ein iSCSI-Ziel erstellt.|
|Verlängerungsanforderung |Der Benutzer hat eine Verlängerung über die zweiwöchige Verbindungszeit hinaus angefordert.|
|Rücksendeanforderung |Der Benutzer hat die Rücksendung der Hardware oder der Datenträger angefordert.|
|Trennen |	Das Trennen der Verbindung für die Hardware oder die Datenträger wurde eingeleitet.|
|Getrennt |	Das Ziel wurde ordnungsgemäß abgehängt.|
|Vernichtet |Die Einheit wurde gemäß unserem Verfahren für HDD-Vernichtung vor Ort unbrauchbar gemacht.|
|Rücksendung durch SoftLayer |	Die Hardware oder die Datenträger wurden verpackt und an die in der ursprünglichen Anforderung angegebene Rücksendeadresse versendet.|
