---

copyright:
  years: 1994, 2017
lastupdated: "2017-12-18"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Datenübertragungsservice - Häufig gestellte Fragen (FAQ)

## Was ist die Datenübertragung?

Mit der Datenübertragung können berechtigte Benutzer (in der Regel der Kontoadministrator) kompatible Einheiten an eines unserer Rechenzentren senden, damit sie direkt mit dem Kontonetz verbunden werden. Die Einheit befindet sich in einem dedizierten Rack im ausgewählten Rechenzentrum und ist für einen Zeitraum von zwei (2) Wochen als iSCSI-Ziel angehängt. In diesem Zeitraum kann der Administrator die Einheit im Netz aufrufen und zusammen mit anderen Einheiten und/oder Services in dem zugehörigen Konto nutzen. Nach Ablauf der zwei Wochen kann eine Verlängerung angefordert werden, damit die Einheit weiterhin mit dem Netz verbunden bleibt. Andernfalls wird die Einheit an die Partei zurückgegeben, die beim Erstellen der Anforderung im Abschnitt für die Rücksendeadresse angegeben wurde, oder die Einheit wird vor Ort vernichtet, wenn keine Rücksendung angefordert wurde.


## Kann ich eine Einheit für Datenübertragung international versenden?

Hardware und Datenträger können an jedes unserer Rechenzentren im In- und Ausland versendet werden. Dabei sind Sie als Kunde für Folgendes verantwortlich:

- Sicherstellen, dass für den Versand der Einheit an das {{site.data.keyword.IBM}} Rechenzentrum oder für die Rücksendung zum Kunden (falls zutreffend) keine Import- oder Exportgenehmigung erforderlich ist.
- Sicherstellen, dass weder für den Kunden noch für etwaige Endbenutzer des Kunden, deren Daten im Inhalt enthalten sind, gesetzliche Bestimmungen in den USA gelten, die ihre bestehenden Exportberechtigungen in den USA aussetzen oder widerrufen. Der Kunde informiert {{site.data.keyword.IBM}} unverzüglich, wenn er selbst oder ein beteiligter Endbenutzer einer solchen gesetzlichen Bestimmung unterliegt.
- Lizenzierung, Transport und Zollabfertigung für die Einheit, einschließlich aller Gebühren, Steuern und Versandkosten zum und vom (falls zutreffend) {{site.data.keyword.IBM}} Rechenzentrum.
- Einhaltung aller anwendbaren Gesetze, einschließlich Datenschutz-, Import- und Exportgesetze, im Zusammenhang mit der Zustellung und Rücksendung der Einheit sowie der Übertragung von Inhalten zum {{site.data.keyword.IBM}} Rechenzentrum.
- Abschließen geeigneter Vereinbarungen und Einholen erforderlicher Genehmigungen beim Endbenutzer des Kunden für alle Endbenutzerdaten, die der Kunde in die Hardware übertragen wird.

Legen Sie Ihrer Sendung ein freigemachtes Rücksendeetikett sowie alle zugehörigen Exportdokumente bei, damit wir die Einheit(en) ordnungsgemäß verpacken, dokumentieren und adressieren können. Wenn keine Rücksendung angefordert wurde, wird die Einheit vernichtet.


## Welche Einheitentypen kann ich mit einer Datenübertragungsanforderung senden?
Halten Sie beim Auswählen einer Einheit oder eines Datenträgers (CD oder DVD) zum Einsenden für die Datenübertragung die folgenden Richtlinien ein:

- Hardwarevoraussetzungen:
   - Die Stromversorgung muss mit einer Spannung von 208 V bzw. 220 V kompatibel sein.

   - Der Netzstecker muss in eine 120 V-Steckdose (NEMA 5-15P) passen.

   - Die Einheit muss mit USB 2.0 oder USB 3.0 kompatibel sein.

   - Ein USB-Stecker (USB-Standardstecker, geeignet für die meisten Computer) muss vorhanden sein.
 
- Voraussetzungen für CD/DVD:

   - Datenträger müssen in CD-Alben, Transportbehältern oder ähnlichen Schutzhüllen eingesandt werden. Verpacken Sie mehrere Datenträger zum Einsenden in einem einzigen Behälter oder CD-Album.

   - Jeder Datenträger muss gut lesbar und eindeutig beschriftet sein (z. B. Datenträger A, Datenträger B, Datenträger C usw.).
   
## Kann meine Einheit beim Datenübertragungsprozess schon vor der zweiwöchigen Frist zurückgesendet oder länger als zwei Wochen aufbewahrt werden? 

Ja, Ihre Hardware oder Datenträger können bei Bedarf an einem beliebigen Zeitpunkt zurückgesandt werden oder über den üblichen Zeitraum hinaus verbunden bleiben. Um eine frühere Rückgabe oder längere Bereitstellung anzufordern, fügen Sie im ursprünglichen Ticket der Datenübertragungsanforderung einen entsprechenden Kommentar hinzu. Wenn die Rücksendung gewünscht ist, entnehmen wir die Hardware bzw. Datenträger aus dem System und senden Sie unter Verwendung der von Ihnen bereitgestellten Verpackung und der freigemachten Versandaufkleber an die Rücksendeadresse, die in der ursprünglichen Anforderung angegeben wurde. 

Jede Verlängerungsanforderung wird schnellstmöglich verarbeitet. Dabei ist zu beachten, dass jede Verlängerungsanforderung die Verbindungszeit der Einheit um eine Woche verlängert. Für den Verlängerungszeitraum werden gegebenenfalls zusätzliche Gebühren berechnet. Weitere Details werden bereitgestellt, wenn ein Mitglied unseres Teams auf die Anforderung in dem ursprünglichen Ticket antwortet.
   
## Was bedeuten die verschiedenen Statusangaben in meinem Datenübertragungsticket?

Jeder Status im Datenübertragungsticket gibt die Phase des Übertragungsprozesses für die Hardware bzw. Datenträger an, die an das Rechenzentrum eingesandt wurden. Weitere Details zu den einzelnen Status enthält die nachfolgende Tabelle:

|Status 	| Definition |
|---------| -----------|
|An SoftLayer gesendet	|Die Datenübertragungsanforderung wurde vom Benutzer abgeschickt und die Hardware bzw. Datenträger werden an das ausgewählte Rechenzentrum ausgeliefert.|
|Von SoftLayer empfangen |	Die Sendung wurde im Rechenzentrum empfangen, unter einer Seriennummer registriert und in unser System eingelesen.|
|Verbunden |	Die Hardware bzw. der Datenträger wurde mit der Einheit verbunden.|
|Bereitgestellt |	Für die Einheit wurde ein iSCSI-Ziel erstellt.|
|Verlängerungsanforderung |	Der Benutzer hat eine Verlängerung über die zweiwöchige Verbindungszeit hinaus angefordert.|
|Rücksendeanforderung | Der Benutzer hat die Rücksendung der Hardware oder des/der Datenträger(s) angefordert.|
|Trennen |	Das Trennen der Verbindung für die Hardware oder den/die Datenträger wurde eingeleitet.|
|Getrennt |	Das Ziel wurde ordnungsgemäß von den Informationssystemen abgehängt.|
|Vernichtet | Die Einheit wurde gemäß unserem Verfahren für HDD-Vernichtung vor Ort unbrauchbar gemacht.|
|Rücksendung durch SoftLayer |	Die Hardware oder Datenträger wurden verpackt und an die in der ursprünglichen Anforderung angegebene Rücksendeadresse versendet.|
