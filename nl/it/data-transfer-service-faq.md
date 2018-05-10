---

copyright:
  years: 1994, 2017
lastupdated: "2017-12-18"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Domande frequenti (FAQ) sul servizio di trasferimento dati

## Cos'è il trasferimento dati?

Il trasferimento dati consente agli utenti autorizzati (di norma l'amministratore dell'account) di inviare dei dispositivi compatibili a uno dei nostri data center perché siano connessi direttamente alla rete dell'account. Il dispositivo è alloggiato in un rack dedicato nel data center selezionato ed è montato come una destinazione iSCSI per un periodo di due (2) settimane. Durante tale periodo, l'amministratore può accedere al dispositivo sulla rete per utilizzarlo con gli altri dispositivi e/o servizi nell'account. Dopo il periodo di due settimane, è possibile richiedere un'estensione per tenere il dispositivo connesso alla rete. In caso contrario, il dispositivo viene restituito alla parte specificata nella sezione relativa all'indirizzo di restituzione quando è stata creata la richiesta; altrimenti, il dispositivo viene distrutto in loco se non è stata richiesta la restituzione.


## Posso fare una spedizione internazionale di un dispositivo per il trasferimento dati?

È possibile fare una spedizione sia domestica che internazionale di hardware e dischi a qualsiasi nostro data center; tuttavia, in quanto cliente, è tua responsabilità:

- assicurarti che non sia necessaria alcuna licenza di importazione o esportazione per spedire il dispositivo al data center {{site.data.keyword.IBM}} o per restituirlo al cliente (se applicabile):
- assicurarti che né il cliente né qualsiasi utente finale del cliente i cui dati sono inclusi nel contenuto siano soggetti a un ordine del governo degli Stati Uniti che revoca o nega loro i privilegi di esportazione statunitensi. Il cliente accetta di informare {{site.data.keyword.IBM}} immediatamente se il cliente stesso o un Suo utente finale diviene oggetto di un tale ordine;
- ottenere tutte le autorizzazioni relative a licenze, spedizione e dogana per il dispositivo, compreso il pagamento di eventuali dazi, imposte e costi di spedizione verso e dal (se applicabile) data center {{site.data.keyword.IBM}};
- rispettare tutte le leggi applicabili, comprese quelle relative alla riservatezza, all'importazione e all'esportazione, associate alla consegna e alla restituzione del dispositivo e al trasferimento del contenuto al data center {{site.data.keyword.IBM}} e
- implementare i corretti accordi e ottenere tutte le autorizzazioni richieste presso l'utente finale del cliente per tutti i dati dell'utente finale che il cliente trasferirà all'hardware.

Includi un'etichetta di spedizione di restituzione prepagata e tutti i documenti di esportazione appropriati con la tua spedizione; noi provvederemo a imballare il dispositivo o i dispositivi per la restituzione utilizzando l'etichetta e i documenti da te forniti. Se la restituzione non è stata richiesta, il dispositivo verrà distrutto.


## Quali tipi di dispositivi posso inviare con una richiesta di trasferimento dati?
Utilizza le seguenti linee guida quando selezioni un dispositivo o un disco (CD o DVD) per l'invio per il trasferimento dati:

- Requisiti hardware:
   - L'alimentazione deve essere compatibile con 208v/220v.

   - La spina di alimentazione deve essere adatta a una presa elettrica a 120v standard (NEMA 5-15P).

   - Il dispositivo deve essere compatibile con USB 2.0 o USB 3.0.

   - fornisci un connettore USB A maschio (presa USB standard adatta alla maggior parte dei computer).
 
- Requisiti CD/DVD

   - I dischi devono essere inviati in custodie di tipo jewel case o astuccio porta CD o in un contenitore simile. Se invii più dischi, mettili insieme in una singola scatola o custodia di tipo astuccio porta CD.

   - Ogni disco deve essere etichettato in modo chiaro ed univoco (ossia Disco A, Disco B, Disco C ecc.).
   
## Posso riavere il mio dispositivo prima, o farlo stare più a lungo, di due settimane durante il processo di trasferimento dati? 

Sì, il tuo hardware o i tuoi dischi possono essere restituiti in qualsiasi momento oppure possono restare connessi più a lungo, se necessario. Per richiedere una restituzione o un'estensione, aggiungi un commento al ticket di richiesta di trasferimento dati originale con la richiesta appropriata. Se richiedi una restituzione, disconnetteremo e restituiremo l'hardware o i dischi all'indirizzo di spedizione di restituzione fornito nella richiesta originale utilizzando le etichette di spedizione prepagate e l'imballaggio da te forniti. 

Se richiedi un'estensione, la richiesta di estensione verrà elaborata il più rapidamente possibile. È importante notare che ciascuna richiesta di estensione estende il tempo per cui il dispositivo è connesso di una settimana e può essere soggetta a un costo di estensione. Ulteriori dettagli verranno inclusi quando un membro del nostro team risponderà alla richiesta nel ticket originale.
   
## Cosa significa ciascuno stato nel mio ticket di trasferimento dati?

Ciascuno stato nel ticket di trasferimento dati indica la fase del processo di trasferimento per l'hardware o i dischi inviati al data center. Fai riferimento alla tabella di seguito per gli specifici dettagli su ciascuno stato:

|Stato | Definizione |
|---------| -----------|
|Sent To SoftLayer 	|La richiesta di trasferimento dati è stata inviata dall'utente ed è in corso la spedizione dell'hardware o dei dischi al data center selezionato.|
|Received by SoftLayer |	La spedizione è stata ricevuta dal data center, le è stato assegnato un numero di serie e ne è stata eseguita la scansione nel nostro sistema.|
|Connect |	L'hardware o il disco sono stati connessi al dispositivo.|
|Connected |	Una destinazione iSCSI è stata creata per il dispositivo.|
|Request for Extension |	L'utente ha richiesto un'estensione del tempo di connessione di due (2) settimane.|
|Request for Return | L'utente ha richiesto la restituzione dell'hardware o dei dischi.|
|Disconnect |	La disconnessione dell'hardware o dei dischi è stata avviata.|
|Disconnected |	La destinazione è stata correttamente scollegata dai sistemi informatici.|
|Destroyed | Il dispositivo è stato distrutto in loco nel rispetto della nostra procedura di distruzione delle unità disco rigido.|
|Return by SoftLayer |	L'hardware o i dischi sono stati imballati e spediti all'indirizzo di restituzione fornito nella richiesta originale.|
