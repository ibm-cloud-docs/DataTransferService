---

copyright:
  years: 1994, 2017
lastupdated: "2017-12-18"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Introduzione al servizio di trasferimento dati

Il servizio di trasferimento dati di {{site.data.keyword.BluSoftlayer_full}} consente ai clienti di inviare un dispositivo compatibile con USB 2.0 o USB 3.0 e/o CD e DVD a un data center {{site.data.keyword.BluSoftlayer}} da connettere direttamente alla relativa rete per controllare in remoto il trasferimento dati. Il dispositivo viene alloggiato in un rack dedicato che si trova nel data center del cliente e verrà montato come una destinazione iSCSI. Il nostro servizio di trasferimento dati è l'ideale quando devi trasferire notevoli quantità di dati senza utilizzare la nostra rete privata ed è un servizio offerto gratuitamente a tutti i clienti {{site.data.keyword.BluSoftlayer}}.

## Accesso alla schermata Data Transfer Service

**Nota**: questa schermata è attualmente disponibile solo all'utente master dell'account.

1. Accedi a [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} utilizzando le tue credenziali univoche.
2. Seleziona **Storage** > **Data Migration** > **Data Transfer** dalla barra di navigazione per accedere alla schermata Data Transfer Service. <br/>

Quando accedono alla schermata Data Transfer Service, gli utenti possono inviare una richiesta di trasferimento dati, visualizzare i dettagli relativi a una richiesta, visualizzare la cronologia dei ticket associata alla traccia del dispositivo per un richiesta e annullare una richiesta esistente.

## Invio di una richiesta di trasferimento dati

Le richieste di trasferimento dati sono state pensate per fare in modo che le parti appropriate nei nostri data center sappiano che devono aspettarsi l'arrivo di una spedizione da un cliente. Le richieste vengono inviata tramite il [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. Quando crei una richiesta, tieni presente le seguenti linee guida:

- Assicurati che il dispositivo oggetto dell'invio in associazione con la richiesta soddisfi tutti i [requisiti hardware](/docs/infrastructure/DataTransferService/data-transfer-service-faq.html).
- A ciascuna richiesta può essere associato solo un singolo dispositivo. Se vuoi inviare più dispositivi, crea una nuova richiesta per ogni dispositivo.
- Se il dispositivo deve essere restituito, fornisci nell'imballaggio un'etichetta di spedizione prepagata e i documenti di esportazione come necessario in modo che il dispositivo possa essere restituito dopo il periodo di trasferimento.
- In caso di spedizione internazionale, è tua responsabilità ottenere tutte le autorizzazioni relative a licenze, spedizione e dogana per il dispositivo, compreso il pagamento di eventuali dazi, imposte e costi di spedizione verso e dal (se applicabile) data center IBM.
- Il corriere e il numero di tracciabilità per la spedizione al nostro data center devono essere forniti quando si completa la richiesta. Assicurati che l'etichetta sia stata creata con l'appropriato indirizzo di data center prima di completare la richiesta.

Attieniti alla procedura di seguito per inviare una richiesta di trasferimento dati.

1. Accedi alla schermata **Data Transfer Service** nel [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. <br/> **Nota**: questa schermata è disponibile solo all'utente master dell'account.
2. Fai clic su **Order Data Transfer Request** nella parte superiore dello schermo.
3. Completa ciascun campo nella sezione **Device Information** in base alla seguente tabella.
<table border="1">
<tbody>
 <tr><th>Nome campo</th><th>Istruzioni</th></tr>
 <tr><td>Device Type</td><td>Il tipo di dispositivo che si sta inviando alla destinazione. Se il tipo di dispositivo non è elencato, seleziona "Other".</td></tr>
 <tr><td>Serial Number</td><td> Il numero di serie per il dispositivo.</td></tr><tr><td>Description</td><td>Una breve descrizione del dispositivo. Dei dettagli importanti da includere possono essere dei fattori identificativi quali il colore, le etichette o gli sticker attaccati ecc.</td></tr>
 <tr><td>Note</td><td>Qualsiasi nota aggiuntiva relativa al dispositivo o al trasferimento.</td></tr><tr><td>Destination</td><td>Il data center che riceverà il dispositivo.</td></tr>
 <tr><td>Carrier</td><td>Corriere postale o espresso utilizzato per spedire il dispositivo alla sua destinazione.</td></tr>
 <tr><td>Tracking Number</td><td>Numero di tracciabilità completo per la spedizione.</td></tr>
 </tbody>
 </table>

4. Completa ciascun campo nella sezione **Return Address** oppure seleziona la casella di spunta **Company Address** per compilare automaticamente i campi con l'indirizzo dell'azienda in archivio. <br/> **Nota**: ricordati di includere nell'imballaggio l'etichetta di spedizione di restituzione prepagata e i documenti di esportazione in modo che il dispositivo possa essere restituito dopo il periodo di trasferimento.
5. Seleziona la casella di spunta **I have read and agree to the Data Transfer Service Agreement and the Master Service Agreement** dopo aver letto ogni accordo di servizio fornito.
6. Fai clic su **Submit Service Request** per inviare la richiesta. Fai clic su **Cancel** per annullare l'azione.

Dopo che hai inviato la richiesta, lo stato del ticket di richiesta si presenterà come *Sent to SoftLayer*. Ti invitiamo a informarci se qualche spedizione di importazione o esportazione richiede una licenza dal tuo governo locale e di allegare le informazioni sulle licenze nel ticket.

Dopo che il dispositivo è stato ricevuto, lo stato viene aggiornato come *Received by SoftLayer* e aggiornato nuovamente come *Connected* dopo che un tecnico del data center ha connesso il dispositivo alla nostra rete. 

Il periodo di trasferimento dati iniziale non deve durare più di due (2) settimane. Durante tale periodo, l'accesso al dispositivo è consentito solo all'amministratore dell'account. Se è necessario del tempo aggiuntivo, è possibile richiedere un'estensione. Viceversa, se il dispositivo deve essere spedito prima che trascorrano le due (2) settimane, è possibile effettuare una richiesta di restituzione. Devi informare {{site.data.keyword.IBM}} tramite il [{{site.data.keyword.slportal}}](https://control.softlayer.com/) dopo che il trasferimento è stato completato. Scollegheremo il dispositivo e lo restituiremo o lo distruggeremo, a seconda di quello che hai richiesto.


## Accesso alla schermata Shipments

La schermata Shipments nel [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} visualizza tutte le spedizioni associate alle richieste del servizio di trasferimento dati. Da questa schermata, è possibile visualizzare le spedizioni e confermare le spedizioni di restituzione alla loro ricezione. Attieniti alla procedura di seguito per accedere alla schermata Shipments.

1. Accedi a [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} utilizzando le tue credenziali univoche.
2. Seleziona **Account** > **Manage** > **Shipments** dalla barra di navigazione per accedere alla schermata Shipments.

Quando accedi alla schermata Shipments, nell'elenco delle spedizioni saranno visualizzate tutte le richieste di spedizione degli ultimi 30 giorni, insieme ai dettagli relativi a ogni singola spedizione. Le spedizioni possono essere [ordinate o filtrate](sort-or-filter-shipments-list.html) in base allo stato, alla data/ora a cui risalgono o a specifici dettagli della spedizione. Inoltre, da questa schermata è possibile confermare la ricezione di spedizioni di restituzione.
![Schermata Shipments](/images/DTSShipmentScreen1.png)
