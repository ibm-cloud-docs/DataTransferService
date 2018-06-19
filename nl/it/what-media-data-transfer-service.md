---

copyright:
  years: 2017, 2018
lastupdated: "2018-05-22"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Cos'è il servizio di trasferimento dati del supporto?
 
Il servizio di trasferimento dati è un servizio che consente di inviare un dispositivo compatibile con USB 2.0 o 3.0, CD e DVD a un data center {{site.data.keyword.BluSoftlayer_full}} da connettere direttamente alla tua rete. Il dispositivo è alloggiato in un rack dedicato ed è montato come una destinazione iSCSI. Sono attualmente supportate anche le unità con formato avanzato.

## Requisiti hardware
1.    Il dispositivo deve avere un'alimentazione compatibile con 208v/220v
2.    Il dispositivo deve avere una spina di alimentazione adatta a una presa elettrica a 120v standard (NEMA 5-15P)
3.    Il dispositivo deve essere compatibile con USB 2.0 (è ora supportata anche la 3.0)
4.    Il dispositivo deve essere provvisto di un cavo USB con connettore USB A maschio (presa standard adatta per la maggior parte dei computer)
5.    CD / DVD
      1.    Devono essere in custodie di tipo jewel case o astuccio porta CD, oppure qualsiasi altro tipo di custodia o contenitore, e preferibilmente tutti insieme in un singolo contenitore (un astuccio porta CD, ad esempio) e ciascun disco deve essere etichettato in maniera univoca.
      2.    Verrà eseguita una rotazione dei dischi su richiesta del cliente tramite il ticket

## Costi a tuo carico
1.    Richiesta iniziale del servizio: $0
2.    Prime 2 settimane di trasferimento dati: $0
      **Nota**: per l'estensione vengono addebitati $25 a settimana.
3.    Il costo di spedizione verso e dal data center {{site.data.keyword.IBM}}, compreso il pagamento di eventuali dazi e imposte.

**Nota**: è responsabilità del cliente:  
- assicurarsi che non sia necessaria alcuna licenza di importazione o esportazione per spedire il dispositivo al data center {{site.data.keyword.IBM}} o per restituirlo al cliente (se applicabile): 
- assicurarsi che il cliente e qualsiasi utente del cliente i cui dati sono inclusi nel contenuto non siano soggetti a un ordine del governo degli Stati Uniti che revoca o nega loro i privilegi di esportazione statunitensi. Informa {{site.data.keyword.IBM}} immediatamente se il cliente stesso o qualsiasi utente come sopra specificato diviene oggetto di un tale ordine;  
- ottenere tutte le autorizzazioni relative a licenze, spedizione e dogana per il dispositivo. Le responsabilità del cliente includono il pagamento di eventuali dazi, imposte e costi di spedizione verso e dal (se applicabile) data center {{site.data.keyword.IBM}}.   
- rispettare tutte le leggi applicabili associate alla consegna e alla restituzione del dispositivo e al trasferimento del contenuto al data center {{site.data.keyword.IBM}} Ciò include quelle relative alla riservatezza, all'importazione e all'esportazione,
- disporre dei corretti accordi con e ottenere tutte le autorizzazioni richieste dall'utente del cliente per gli eventuali dati dell'utente che il cliente desidera trasferire all'hardware.

## Come effettuare una richiesta
Tale operazione viene eseguita in **Storage** > **Data Migration** > **Data Transfer** facendo clic su **Order Data Transfer Request** nell'angolo in alto a destra.

![Come effettuare una richiesta di trasferimento dati](/images/DTS.png)

Completa il modulo con i seguenti dati del dispositivo
1. Numero di serie
2. Il tipo
3. Una breve descrizione del dispositivo
4. Il data center a cui desideri vada il dispositivo
5. Il numero di tracciabilità utilizzato per tracciare la spedizione
6. Il servizio di corriere utilizzato
7. L'indirizzo di restituzione a cui si desidera venga spedito il dispositivo quando finisce il periodo di trasferimento.

Questa richiesta crea automaticamente un ticket di supporto per avvisare i nostri tecnici che il dispositivo sta per essere spedito e consentire loro di tracciare la consegna. Quando riceviamo il dispositivo, lo connettiamo al nostro rack dedicato. Dopo che abbiamo connesso il dispositivo, il ticket viene aggiornato per fornirti un link alle tue credenziali di accesso alla destinazione iSCSI.

## Richiesta della restituzione
Se hai fornito un indirizzo di restituzione e hai incluso l'etichetta di spedizione prepagata nell'imballaggio, puoi richiedere che il dispositivo ti venga restituito in qualsiasi momento durante il periodo di trasferimento di due settimane. Puoi eseguire questa operazione tramite il [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. Seleziona **Storage** > **Data Migration** > **Data Transfer** e, dal menu **Action** del tuo dispositivo, seleziona **request return**. Questo avvisa i nostri tecnici che desideri che il dispositivo venga disconnesso e che ti venga rispedito.

## Richiesta di un'estensione
Dopo il tuo periodo gratuito di due settimane, se hai ancora bisogno di usare il nostro dispositivo, devi richiedere un'estensione. Questo avvisa i nostri tecnici che desideri estendere il tempo di connessione del dispositivo. Puoi farlo in nello stesso modo in cui richiederesti la restituzione del tuo dispositivo. Seleziona **Storage** > **Data Migration** > **Data Transfer** e, nel menu **Action** per il dispositivo, seleziona **request extension**. Ogni settimana extra comporta un costo di servizio di $25 che deve essere pagato. Nota: la tua richiesta di estensione potrebbe essere negata, a seconda dello spazio disponibile nel data center. Quando la richiesta viene accolta, il ticket viene aggiornato di conseguenza.

## Disconnessione
Dopo il periodo di due settimane, il dispositivo viene disconnesso automaticamente dal nostro data center. Se hai richiesto una restituzione, il tuo dispositivo ti viene restituito dal corriere da te scelto e all'indirizzo di restituzione da te specificato nella richiesta iniziale. Il ticket viene aggiornato indicando che il dispositivo è stato disconnesso. Se non hai richiesto la restituzione del tuo dispositivo, si provvede alla sua distruzione in loco.
