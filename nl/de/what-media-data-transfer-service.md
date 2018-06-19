---

copyright:
  years: 2017, 2018
lastupdated: "2018-05-22"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Was ist der Data Transfer-Service für Mediendaten?
 
Mit dem Data Transfer-Service können Sie eine USB 2.0- oder USB 3.0-kompatible Einheit, CDs und DVDs an ein {{site.data.keyword.BluSoftlayer_full}}-Rechenzentrum senden, die direkt mit Ihrem Netz verbunden werden sollen. Die Einheit befindet sich in einem dedizierten Rack und ist als iSCSI-Ziel angehängt. Laufwerke mit erweitertem Format (Advanced Format) werden jetzt ebenfalls unterstützt.

## Hardwarevoraussetzungen
1.    Die Stromversorgung der Einheit muss mit einer Spannung von 208 V bzw. 220 V kompatibel sein.
2.    Der Netzstecker der Einheit muss in eine 120 V-Steckdose (NEMA 5-15P) passen.
3.    Die Einheit muss mit USB 2.0 kompatibel sein (USB 3.0 wird jetzt ebenfalls unterstützt).
4.    Die Einheit muss mit einem USB-Kabel mit USB A-Stecker (Standardstecker, geeignet für die meisten Computer) ausgestattet sein.
5.    CDs / DVDs
      1.    Müssen in CD-Alben, Hüllen, Transportbehälter oder einen anderen Behälter eingelegt sein, möglichst nur ein Behälter (z. B. CD-Album) für alle CDs, und jeder Datenträger muss eindeutig beschriftet sein.
      2.    Die Datenträger werden auf Anforderung des Kunden turnusmäßig gewechselt, wie im Ticket angegeben.

## Anfallende Kosten
1.    Ursprüngliche Serviceanforderung: Kostenfrei
2.    Erste zwei Wochen für Data Transfer: Kostenfrei
      **Hinweis**: $ 25 pro Woche für jede Verlängerung
3.    Versandkosten zum und vom {{site.data.keyword.IBM}}-Rechenzentrum einschließlich Gebühren und Steuern.

**Hinweis**: Der Kunde ist für Folgendes verantwortlich:  
- Sicherstellen, dass für den Versand der Einheit an das {{site.data.keyword.IBM}} Rechenzentrum oder für die Rücksendung zum Kunden (falls zutreffend) keine Import- oder Exportgenehmigung erforderlich ist. 
- Sicherstellen, dass weder für den Kunden noch für etwaige Benutzer des Kunden, deren Daten im Inhalt enthalten sind, gesetzliche Bestimmungen in den USA gelten, die ihre bestehenden Exportberechtigungen in den USA aussetzen oder widerrufen. Der Kunde informiert {{site.data.keyword.IBM}} unverzüglich, wenn er selbst oder ein beteiligter Benutzer einer solchen gesetzlichen Bestimmung unterliegt.  
- Lizenzierung, Transport und Zollabfertigung für die Einheit, einschließlich aller Gebühren, Steuern und Versandkosten zum und vom {{site.data.keyword.IBM}} Rechenzentrum (falls zutreffend).   
- Einhaltung aller anwendbaren Gesetze im Zusammenhang mit der Zustellung und Rücksendung der Einheit sowie der Übertragung von Inhalten zum {{site.data.keyword.IBM}} Rechenzentrum. Dies schließt Datenschutz-, Import- und Exportgesetze ein.
- Abschließen geeigneter Vereinbarungen und Einholen erforderlicher Genehmigungen beim Benutzer des Kunden für alle Benutzerdaten, die der Kunde in die Hardware übertragen möchte.

## Anforderung erstellen
Wählen Sie hierzu **Speicher** > **Datenmigration** >  **Data Transfer** aus und klicken Sie dann auf **Data Transfer-Anforderung bestellen** in der rechten oberen Ecke der Seite.

![Data Transfer-Anforderung erstellen](/images/DTS.png)

Füllen Sie das Formular mit den folgenden Angaben für die Einheit aus:
1. Seriennummer
2. Typ
3. Kurzbeschreibung der Einheit
4. Rechenzentrum, in dem die Einheit bereitgestellt werden soll
5. Tracking-Nummer für die Sendungsverfolgung
6. Beauftragter Zusteller
7. Rücksendeadresse für die Einheit nach Abschluss des Übertragungszeitraums

Mit dieser Anforderung wird ein Support-Ticket erstellt, um unseren Techniker über den Versand der Einheit zu informieren und die Sendungsverfolgung zu ermöglichen. Nach der Zustellung wird die Einheit von uns an das dedizierte Rack angeschlossen. Nach dem Verbinden der Einheit wird das Ticket aktualisiert und enthält einen Link, über den Sie Ihre Anmeldeberechtigungsnachweise für das iSCSI-Ziel aufrufen können.

## Rücksendung anfordern
Wenn Sie eine Rücksendeadresse angegeben und Ihrer Sendung einen freigemachten Versandaufkleber beigelegt haben, können Sie anfordern, dass die Einheit nach dem zweiwöchigen Übertragungszeitraum an Sie zurück gesendet wird. Dies erfolgt über das [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. Wählen Sie **Speicher** > **Datenmigration** > **Data Transfer** und im Menü **Aktion** für Ihre Einheit die Option **Rücksendung anfordern** aus. Daraufhin werden unsere Techniker informiert, dass Ihre Einheit aus dem System entfernt und an Sie zurück gesendet werden soll.

## Verlängerung anfordern
Wenn Ihre Einheit über die kostenlose zweiwöchige Frist hinaus bereitgestellt werden soll, müssen Sie eine Verlängerung anfordern. Daraufhin werden unsere Techniker informiert, dass Ihre Einheit länger verbunden bleiben soll. Dies geschieht auf die gleiche Weise wie das Anfordern der Rücksendung der Einheit. Wählen Sie **Speicher** > **Datenmigration** > **Data Transfer** und im Menü **Aktion** für Ihre Einheit die Option **Verlängerung anfordern** aus. Für jede zusätzliche Woche fällt eine Servicegebühr von $ 25 an. Beachten Sie, dass Ihre Verlängerungsanforderung abgelehnt werden kann. Dies ist vom verfügbaren Speicherplatz im Rechenzentrum abhängig. Wenn die Anforderung genehmigt wird, wird das Ticken entsprechend aktualisiert.

## Verbindung trennen
Nach einem Zeitraum von zwei Wochen wird die Verbindung der Einheit zum Rechenzentrum automatisch getrennt. Wenn Sie eine Rücksendung angefordert haben, wird Ihre Einheit über den von Ihnen ausgewählten Zusteller an die in der ursprünglichen Anforderung angegebene Rücksendeadresse zurückgesandt. Das Ticket wird aktualisiert und gibt an, dass die Verbindung für die Einheit getrennt wurde. Wenn Sie keine Rücksendung angefordert haben, wird die Einheit vernichtet.
