---

copyright:
  years: 2017
lastupdated: "2017-12-18"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Was ist der Übertragungsservice für Mediendaten
 
Mit dem Datenübertragungsservice können Sie eine USB 2.0- oder USB 3.0-kompatible Einheit und/oder CDs und DVDs an ein {{site.data.keyword.BluSoftlayer_full}}-Rechenzentrum senden, die direkt mit Ihrem Netz verbunden werden sollen. Die Einheit wird in ein dediziertes Rack in dem ausgewählten Rechenzentrum eingelegt und als iSCSI-Ziel angehängt. Laufwerke mit erweitertem Format (Advanced Format) werden jetzt ebenfalls unterstützt.

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
2.    Erste zwei Wochen der Datenübertragung: Kostenfrei
      **Hinweis**: $ 25 pro Woche für jede Verlängerung
3.    Versandkosten zum und vom {{site.data.keyword.IBM}}-Rechenzentrum einschließlich Gebühren und Steuern.

**Hinweis**: Der Kunde ist für Folgendes verantwortlich:  
- Sicherstellen, dass für den Versand der Einheit an das {{site.data.keyword.IBM}} Rechenzentrum oder für die Rücksendung zum Kunden (falls zutreffend) keine Import- oder Exportgenehmigung erforderlich ist. 
- Sicherstellen, dass weder für den Kunden noch für etwaige Endbenutzer des Kunden, deren Daten im Inhalt enthalten sind, gesetzliche Bestimmungen in den USA gelten, die ihre bestehenden Exportberechtigungen in den USA aussetzen oder widerrufen. Der Kunde informiert {{site.data.keyword.IBM}} unverzüglich, wenn er selbst oder ein beteiligter Endbenutzer einer solchen gesetzlichen Bestimmung unterliegt.  
- Lizenzierung, Transport und Zollabfertigung für die Einheit, einschließlich aller Gebühren, Steuern und Versandkosten zum und vom {{site.data.keyword.IBM}} Rechenzentrum (falls zutreffend).   
- Einhaltung aller anwendbaren Gesetze, einschließlich Datenschutz-, Import- und Exportgesetze, im Zusammenhang mit der Zustellung und Rücksendung der Einheit sowie der Übertragung von Inhalten zum {{site.data.keyword.IBM}} Rechenzentrum. 
- Abschließen geeigneter Vereinbarungen und Einholen erforderlicher Genehmigungen beim Endbenutzer des Kunden für alle Endbenutzerdaten, die der Kunde in die Hardware übertragen wird.

## Anforderung erstellen
Wählen Sie **Storage** > **Datenmigration** >  **Datenübertragung** aus und klicken Sie anschließend auf den Link **Datenübertragungsanforderung bestellen** in der rechten oberen Ecke der Seite.

![Datenübertragungsanforderung erstellen](/images/DTS.png)
 

Geben Sie in diesem Formular folgende Details zu der Einheit an:
1. Seriennummer
2. Typ
3. Kurzbeschreibung der Einheit
4. Rechenzentrum, in dem die Einheit bereitgestellt werden soll
5. Tracking-Nummer für die Sendungsverfolgung
6. Beauftragter Zusteller
7. Rücksendeadresse für die Einheit nach Abschluss des Übertragungszeitraums

Nach Eingabe dieser Daten wird automatisch ein Support-Ticket erstellt, um unseren Techniker über den Versand der Einheit zu informieren und die Sendungsverfolgung zu ermöglichen. Nach der Zustellung wird die Einheit von uns an das dedizierte Rack angeschlossen. Anschließend wird das Ticket aktualisiert und Sie können über einen bereitgestellten Link Ihre Anmeldedaten für das iSCSI-Ziel aufrufen.

## Rücksendung anfordern
Wenn Sie eine Rücksendeadresse angegeben und Ihrer Sendung einen freigemachten Versandaufkleber beigelegt haben, können Sie anfordern, dass die Einheit nach dem zweiwöchigen Übertragungszeitraum an Sie zurück gesendet wird. Zu diesem Zweck wählen Sie im [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} die Optionen **Storage** > **Datenmigration** > **Datenübertragung** und anschließend im Dropdown-Menü **Aktion** für Ihre Einheit die Option **Rücksendung anfordern** aus. Daraufhin werden unsere Techniker informiert, dass Ihre Einheit aus dem System entfernt und an Sie zurück gesendet werden soll.

## Verlängerung anfordern
Wenn Ihre USB-Einheit über die kostenlose zweiwöchige Frist hinaus bereitgestellt werden soll, müssen Sie eine Verlängerung anfordern, damit unsere Techniker informiert werden, dass Ihre Einheit länger verbunden bleiben soll. Dies geschieht auf die gleiche Weise wie das Anfordern der Rücksendung der Einheit, indem Sie **Storage** > **Datenmigration** > **Datenübertragung** und anschließend im Dropdown-Menü **Aktion** für die Einheit die Option **Verlängerung anfordern** auswählen. Für jede weitere Woche nach Ablauf der zwei kostenfreien Wochen, wird eine Gebühr von 25 US-Dollar fällig. Falls die Einheitenkapazitäten im jeweiligen Rechenzentrum nicht ausreichen, wird Ihre Anforderung möglicherweise abgelehnt. Sobald die Anforderung genehmigt ist, wird das Ticket mit der Angabe aktualisiert, dass die Verlängerung um eine Woche gewährt wurde.

## Verbindung trennen
Nach Ablauf des zweiwöchigen Bereitstellungszeitraums wird die Einheit in unserem Rechenzentrum automatisch abgeschaltet und über den angegebenen Zusteller an die Rücksendeadresse zurückgesandt, die Sie in der ursprünglichen Anforderung angegeben haben. Das Ticket wird mit der Angabe aktualisiert, dass die Verbindung der Einheit getrennt wurde. Wenn Sie keine Rücksendung angefordert haben, wird die Einheit vernichtet.
