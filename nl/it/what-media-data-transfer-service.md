---

copyright:
  years: 2017, 2019
lastupdated: "2019-02-05"

---
{:new_window: target="_blank"}

# Introduzione al servizio di trasferimento dati del supporto
{: #mediaDTS}

Con il servizio di trasferimento dati, puoi inviare un dispositivo compatibile con USB 2.0 o 3.0, CD e DVD a un data center {{site.data.keyword.BluSoftlayer_full}} da connettere direttamente alla tua rete. Il dispositivo è alloggiato in un rack dedicato ed è montato come una destinazione iSCSI. Sono attualmente supportate anche le unità con formato avanzato.

## Requisiti hardware
1.    Il dispositivo deve avere un'alimentazione compatibile con 208v/220v
2.    Il dispositivo deve avere una spina di alimentazione adatta a una presa elettrica a 120v standard (NEMA 5-15P)
3.    Il dispositivo deve essere compatibile con USB 2.0 (è ora supportata anche la 3.0)
4.    Il dispositivo deve essere provvisto di un cavo USB con connettore USB A maschio (presa standard adatta per la maggior parte dei computer)
5.    CD / DVD
      - Devono essere in custodie di tipo jewel case o astuccio porta CD, oppure qualsiasi altro tipo di custodia o contenitore. È possibile posizionarli tutti insieme in un singolo contenitore (un astuccio porta CD, ad esempio). Ciascun disco deve essere etichettato in maniera univoca.
      - I dischi vengono ruotati su richiesta del cliente tramite il ticket.

## Costi a tuo carico
1.    Richiesta iniziale del servizio = $0
2.    Prime 2 settimane di trasferimento dati = $0
      **Nota**: per l'estensione vengono addebitati $25 a settimana.
3.    Il costo di spedizione verso e dal data center {{site.data.keyword.IBM}}, compreso il pagamento di eventuali dazi e imposte.

**Nota**: è responsabilità del cliente
- Assicurarti che non sia necessaria alcuna licenza di importazione o esportazione per spedire il dispositivo al data center {{site.data.keyword.IBM}} o per restituirlo al cliente (se applicabile).
- Assicurarsi che il cliente e qualsiasi utente del cliente i cui dati sono inclusi nel contenuto non siano soggetti a un ordine del governo degli Stati Uniti che revoca o nega loro i privilegi di esportazione statunitensi. Informa {{site.data.keyword.IBM}} immediatamente se il cliente stesso o qualsiasi utente come sopra specificato diviene oggetto di un tale ordine.
- Ottenere tutte le autorizzazioni relative a licenze, spedizione e dogana per il dispositivo. Le responsabilità del cliente includono il pagamento di eventuali dazi, imposte e costi di spedizione verso e dal (se applicabile) data center {{site.data.keyword.IBM}}.
- Rispettare tutte le leggi applicabili associate alla consegna e alla restituzione del dispositivo e al trasferimento del contenuto al data center {{site.data.keyword.IBM}} Questo requisito include quelle relative alla riservatezza, all'importazione e all'esportazione,
- Disporre dei corretti accordi con e ottenere tutte le autorizzazioni richieste dall'utente del cliente per gli eventuali dati dell'utente che il cliente desidera trasferire all'hardware.

## Come effettuare una richiesta
Puoi inoltrare una richiesta tramite il [{{site.data.keyword.slportal}} ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){:new_window}

1. Fai clic su **Storage** > **Data Migration** > **Data Transfer**.
2. Fai clic su **Order Data Transfer Request**.

![Come effettuare una richiesta di trasferimento dati](/images/DTS.png)

Completa il modulo con i seguenti dati del dispositivo
1. Numero di serie
2. Il tipo
3. Una breve descrizione del dispositivo
4. Il data center a cui desideri vada il dispositivo
5. Il numero di tracciabilità utilizzato per tracciare la spedizione
6. Il servizio di corriere utilizzato
7. Indirizzo di ritorno del punto in cui desideri che il dispositivo venga inviato dopo che il trasferimento dei dati è terminato.

Questa richiesta crea automaticamente un ticket di supporto per avvisare i tecnici {{site.data.keyword.BluSoftlayer}} che il dispositivo sta per essere spedito e consentire loro di tracciare la consegna. Quando {{site.data.keyword.BluSoftlayer}} riceve il dispositivo, i tecnici si collegano ad esso nel rack dedicato. Quando il dispositivo è collegato, il ticket viene aggiornato per fornirti un link alle tue credenziali di accesso alla destinazione iSCSI.

## Richiesta di una restituzione
Se hai fornito un indirizzo di restituzione e hai incluso l'etichetta di spedizione prepagata nell'imballaggio, puoi richiedere che il dispositivo ti venga restituito in qualsiasi momento durante il periodo di trasferimento di due settimane. Puoi inoltrare la richiesta tramite il [{{site.data.keyword.slportal}} ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){:new_window}.

1. Seleziona **Storage** > **Data Migration** > **Data Transfer**.
2. Dal menu **Action** del tuo dispositivo, seleziona **request return**.

Questo avvisa i tecnici {{site.data.keyword.BluSoftlayer}} che desideri che il dispositivo venga disconnesso e che ti venga rispedito.

## Richiesta di un'estensione
Dopo il tuo periodo gratuito di due settimane, se hai ancora bisogno di usare il nostro dispositivo, devi richiedere un'estensione tramite il [{{site.data.keyword.slportal}} ![Icona link esterno](../../icons/launch-glyph.svg "Icona link esterno")](https://control.softlayer.com/){:new_window}. Questo avvisa i tecnici {{site.data.keyword.BluSoftlayer}} che desideri estendere il tempo di connessione del dispositivo.

1. Seleziona **Storage** > **Data Migration** > **Data Transfer**
2. Nel menu **Action** per il dispositivo, seleziona **request extension**.

Ogni settimana extra comporta un costo di servizio di $25 che deve essere pagato. La tua richiesta di estensione potrebbe essere negata, a seconda dello spazio disponibile nel data center. Quando la richiesta viene accolta, il ticket viene aggiornato.

## Disconnessione del dispositivo
Dopo il periodo di due settimane, il dispositivo viene disconnesso automaticamente dal data center. Se hai richiesto una restituzione, il tuo dispositivo ti viene restituito dal corriere da te scelto e all'indirizzo di restituzione da te specificato nella richiesta iniziale. Il ticket viene aggiornato indicando che il dispositivo è stato disconnesso. Se non hai richiesto la restituzione del tuo dispositivo, si provvede alla sua distruzione in loco.
