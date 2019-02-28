---

copyright:
  years: 2017, 2019
lastupdated: "2019-02-05"

---
{:faq: data-hd-content-type='faq'}

# Domande frequenti (FAQ)

## Cos'è il trasferimento dati?
{: faq}

Questo servizio consente agli utenti autorizzati (di norma l'amministratore dell'account) di inviare dei dispositivi compatibili a uno dei data center {{site.data.keyword.BluSoftlayer_full}} perché siano connessi direttamente alla rete dell'account. Il dispositivo è alloggiato in un rack dedicato ed è montato come una destinazione iSCSI per due settimane. Durante tale periodo, l'amministratore può accedere al dispositivo sulla rete per utilizzarlo con gli altri dispositivi e servizi nell'account. Dopo il periodo di due settimane, è possibile richiedere un'estensione per tenere il dispositivo connesso alla rete. In caso contrario, il dispositivo viene restituito alla parte specificata nella richiesta oppure viene distrutto in loco.

## Posso fare una spedizione internazionale di un dispositivo per il trasferimento dati?
{: faq}

È possibile fare una spedizione sia domestica che internazionale di hardware e dischi a qualsiasi data center {{site.data.keyword.BluSoftlayer}}. Tuttavia, in quanto cliente, è tua responsabilità:

- Assicurarti che non sia necessaria alcuna licenza di importazione o esportazione per spedire il dispositivo al data center {{site.data.keyword.IBM}} o per restituirlo al cliente (se applicabile):
- Assicurarsi che il cliente e qualsiasi utente del cliente i cui dati sono inclusi nel contenuto non siano soggetti a un ordine del governo degli Stati Uniti che revoca o nega loro i privilegi di esportazione statunitensi. Devi informare {{site.data.keyword.IBM}} immediatamente se la tua azienda o qualsiasi utente come sopra specificato diviene oggetto di un tale ordine;
- Ottenere tutte le autorizzazioni relative a licenze, spedizione e dogana per il dispositivo, compreso il pagamento di eventuali dazi, imposte e costi di spedizione verso e dal (se applicabile) data center {{site.data.keyword.IBM}};
- Rispettare tutte le leggi applicabili, comprese quelle relative alla riservatezza, all'importazione e all'esportazione, associate alla consegna e alla restituzione del dispositivo e al trasferimento del contenuto al data center {{site.data.keyword.IBM}} e
- Implementare i corretti accordi e ottenere tutte le autorizzazioni richieste presso l'utente del cliente per tutti i dati dell'utente che il cliente trasferisce all'hardware.

Includi un'etichetta di spedizione di restituzione prepagata e tutti i documenti di esportazione appropriati con la tua spedizione. {{site.data.keyword.BluSoftlayer}} imballa il dispositivo per la restituzione utilizzando l'etichetta e i documenti da te forniti. Se la restituzione non viene richiesta, il dispositivo viene distrutto.


## Quali tipi di dispositivi posso essere inviati con una richiesta di trasferimento dati?
{: faq}

Utilizza le seguenti linee guida quando selezioni un dispositivo o un disco (CD o DVD) per l'invio per il trasferimento dati:

- **Requisiti hardware**

   - L'alimentazione deve essere compatibile con 208v/220v.

   - La spina di alimentazione deve essere adatta a una presa elettrica a 120v standard (NEMA 5-15P).

   - Il dispositivo deve essere compatibile con USB 2.0 o USB 3.0.

   - fornisci un connettore USB A maschio (presa USB standard adatta alla maggior parte dei computer).

- **Requisiti CD/DVD**

   - I dischi devono essere inviati in custodie di tipo jewel case o astuccio porta CD o in un contenitore simile. Se vuoi inviare più dischi, mettili insieme in una singola scatola o custodia di tipo astuccio porta CD.

   - Ogni disco deve essere etichettato in modo chiaro ed univoco.

## È possibile riavere il dispositivo prima, o farlo stare più a lungo, di due settimane?
{: faq}

Sì, il tuo hardware o i tuoi dischi possono essere restituiti in qualsiasi momento oppure possono restare connessi più a lungo, se necessario. Per richiedere una restituzione o un'estensione, aggiungi un commento al ticket di richiesta di trasferimento dati originale con la richiesta appropriata. Se richiedi una restituzione, {{site.data.keyword.BluSoftlayer}} disconnette e restituisce l'hardware o i dischi all'indirizzo di restituzione fornito nella richiesta originale utilizzando le etichette di spedizione prepagate e l'imballaggio da te forniti.

Se richiedi un'estensione, la richiesta di estensione verrà elaborata il più rapidamente possibile. È importante notare che ciascuna richiesta di estensione estende il tempo per cui il dispositivo è connesso di una settimana e può essere soggetta a un costo di estensione. Ulteriori dettagli verranno inclusi quando un membro del team {{site.data.keyword.BluSoftlayer_full}} risponderà alla richiesta nel ticket originale.

Ciascuno stato nel ticket di trasferimento dati indica la fase del processo di trasferimento per l'hardware o i dischi inviati al data center. Fai riferimento alla tabella per gli specifici dettagli su ciascuno stato:

|Stato 	| Definizione |
|---------| -----------|
|`Sent To SoftLayer` |La richiesta di trasferimento dati è stata inviata dall'utente ed è in corso la spedizione dell'hardware o dei dischi al data center selezionato.|
|`Received by SoftLayer` |	La spedizione è stata ricevuta dal data center, al dispositivo è stato assegnato un numero di serie e ne è stata eseguita la scansione nel sistema {{site.data.keyword.BluSoftlayer}}.|
|`Connect` |	L'hardware o il disco sono connessi al dispositivo.|
|`Connected` |	Una destinazione iSCSI viene creata per il dispositivo.|
|`Request for Extension` | Il cliente ha richiesto un'estensione del tempo di connessione di due settimane.|
|`Request for Return` | Il cliente ha richiesto la restituzione dell'hardware o dei dischi.|
|`Disconnect` |	La disconnessione dell'hardware o dei dischi è stata avviata.|
|`Disconnected` |	La destinazione è stata scollegata correttamente.|
|`Destroyed` | Il dispositivo è stato distrutto in loco nel rispetto della procedura di distruzione delle unità disco rigido {{site.data.keyword.BluSoftlayer}}.|
|`Return by SoftLayer` |	L'hardware o i dischi sono stati imballati e spediti all'indirizzo di restituzione fornito nella richiesta originale.|
