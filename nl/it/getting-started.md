---

copyright:
  years: 2017, 2019
lastupdated: "2019-02-05"

---
{:new_window: target="_blank"}

# Introduzione al servizio di trasferimento dati
{: #gettingstarted}

I clienti possono utilizzare il servizio di trasferimento dati {{site.data.keyword.BluSoftlayer_full}} per inviare un dispositivo compatibile con USB 2.0 o USB 3.0, CD e DVD a un data center {{site.data.keyword.BluSoftlayer}}. Il loro dispositivo viene collegato direttamente alla loro rete in modo che possono controllare in remoto il trasferimento dati. Il dispositivo viene alloggiato in un rack dedicato che si trova nel data center del cliente e viene montato come una destinazione iSCSI. Il servizio di trasferimento dati è l'ideale quando devi trasferire notevoli quantità di dati senza utilizzare la rete privata di {{site.data.keyword.BluSoftlayer}} ed è un servizio offerto gratuitamente a tutti i clienti {{site.data.keyword.BluSoftlayer}}.

## Accesso alla schermata Data Transfer Service

**Nota**: questa schermata è disponibile solo all'utente master dell'account.

1. Accedi al [{{site.data.keyword.slportal}} ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){:new_window} con le tue credenziali univoche.
2. Seleziona **Storage** > **Data Migration** > **Data Transfer** dalla barra di navigazione per accedere alla schermata Data Transfer Service. <br/>

Nella schermata **Data Transfer Service**, gli utenti possono inviare una richiesta di trasferimento dati, visualizzare i dettagli di una richiesta, visualizzare la cronologia dei ticket associata alla traccia del dispositivo e annullare una richiesta esistente.

## Invio di una richiesta di trasferimento dati

Le richieste di trasferimento dati sono state pensate per fare in modo che le parti appropriate nei nostri data center sappiano che devono aspettarsi l'arrivo di una spedizione da un cliente. Le richieste vengono inoltrate tramite il [{{site.data.keyword.slportal}} ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){:new_window}.

Quando crei una richiesta, tieni presente le seguenti linee guida.

- Assicurati che il dispositivo che vuoi inviare soddisfi tutti i [requisiti hardware](/docs/infrastructure/DataTransferService/data-transfer-service-faq.html).
- A una singola richiesta può essere associata solo un singolo dispositivo. Se vuoi inviare più dispositivi, devi creare una nuova richiesta per ogni dispositivo.
- Se il dispositivo deve essere restituito, fornisci nell'imballaggio un'etichetta di spedizione prepagata e i documenti di esportazione come necessario in modo che il dispositivo possa essere restituito dopo il periodo di trasferimento.
- In caso di spedizione internazionale, è tua responsabilità ottenere tutte le autorizzazioni relative a licenze, spedizione e dogana per il dispositivo. Le tue responsabilità includono il pagamento di eventuali dazi, imposte e costi di spedizione verso e dal (se applicabile) data center {{site.data.keyword.BluSoftlayer}}.
- Quando completi la richiesta, devi fornire il nome del corriere e il numero di tracciabilità per la spedizione al data center.  Crea l'etichetta di spedizione con l'appropriato indirizzo del data center prima di inviare la richiesta di trasferimento dati.

Attieniti a questa procedura per inviare una richiesta di trasferimento dati.

1. Accedi alla schermata **Data Transfer Service** nel [{{site.data.keyword.slportal}} ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){:new_window}.
2. Fai clic su **Order Data Transfer Request**.
3. Completa ciascun campo nella sezione **Device Information** in base alla tabella 1.
<table border="1">
<caption>La tabella 1 elenca i nomi dei campi nel modulo di richiesta sulla sinistra e la loro descrizione sulla destra.</caption>
 <tr><th>Nome campo</th><th>Istruzioni</th></tr>
 <tr><td>Device Type</td><td>Il tipo di dispositivo che viene inviato alla destinazione. Se il tipo di dispositivo non è elencato, seleziona "Other".</td></tr>
 <tr><td>Serial Number</td><td> Il numero di serie per il dispositivo.</td></tr><tr><td>Description</td><td>Una breve descrizione del dispositivo. Dei dettagli importanti da includere possono essere dei fattori identificativi quali il colore, le etichette o gli sticker.</td></tr>
 <tr><td>Note</td><td>Qualsiasi nota aggiuntiva relativa al dispositivo o al trasferimento.</td></tr><tr><td>Destination</td><td>Il data center che riceve il dispositivo.</td></tr>
 <tr><td>Carrier</td><td>Corriere postale o espresso utilizzato per spedire il dispositivo alla sua destinazione.</td></tr>
 <tr><td>Tracking Number</td><td>Numero di tracciabilità completo per la spedizione.</td></tr>
 </table>

4. Completa ciascun campo nella sezione **Return Address** oppure seleziona la casella di spunta **Company Address** per compilare automaticamente i campi con l'indirizzo dell'azienda in archivio. <br/> **Nota**: ricordati di includere nell'imballaggio l'etichetta di restituzione prepagata e gli eventuali documenti di esportazione necessari nel pacchetto.
5. Dopo aver letto l'accordo di servizio, seleziona la casella di spunta **I have read and agree to the Data Transfer Service Agreement and the Master Service Agreement**.
6. Fai clic su **Submit Service Request**.

Dopo che hai inviato la richiesta, lo stato del ticket di richiesta si presenta come `Sent to SoftLayer`. Se qualche spedizione di importazione o esportazione richiede una licenza dal tuo governo locale, informa {{site.data.keyword.BluSoftlayer}} e allega le informazioni sulle licenze nel ticket.

Dopo che il dispositivo è stato ricevuto, lo stato viene aggiornato come `Received by SoftLayer`. Lo stato del ticket viene aggiornato nuovamente come `Connected` dopo che un tecnico del data center ha connesso il dispositivo alla rete.

Il periodo di trasferimento dati iniziale è di due settimane. Durante tale periodo, l'accesso al dispositivo è concesso solo all'amministratore dell'account. Se hai bisogno di più tempo, puoi richiedere un'estensione. Inoltre, se vuoi che il dispositivo venga spedito prima delle due settimane, puoi richiedere la restituzione. Devi informare {{site.data.keyword.IBM}} tramite il [{{site.data.keyword.slportal}}](https://control.softlayer.com/) quando il trasferimento è completo. Poi, {{site.data.keyword.BluSoftlayer}} scollega il dispositivo e lo restituisce o distrugge a seconda di quello che hai richiesto.


## Accesso alla schermata Shipments

La schermata Shipments nel [{{site.data.keyword.slportal}} ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){:new_window} visualizza tutte le spedizioni associate alle richieste del servizio di trasferimento dati. Da questa schermata, puoi visualizzare le spedizioni e, al ricevimento, puoi confermare le spedizioni di restituzione.

Per accedere alla schermata Shipments:

1. Accedi al [{{site.data.keyword.slportal}} ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){:new_window} utilizzando le tue credenziali univoche.
2. Seleziona **Account** > **Manage** > **Shipments** dalla barra di navigazione.

Nella schermata Shipments, tutte le richieste di spedizione negli ultimi 30 giorni vengono visualizzate con i relativi dettagli. Le spedizioni possono essere [ordinate o filtrate](sort-or-filter-shipments-list.html) in base allo stato, alla data/ora a cui risalgono o a specifici dettagli della spedizione. In questa schermata puoi inoltre confermare la ricezione di spedizioni di restituzione.
![Schermata Shipments](/images/DTSShipmentScreen1.png)
