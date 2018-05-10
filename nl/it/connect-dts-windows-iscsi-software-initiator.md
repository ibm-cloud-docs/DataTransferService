---

copyright:
  years: 2017
lastupdated: "2017-11-13"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Connessione a un dispositivo DTS in Windows con iSCSI Software Initiator

Per interagire con una LUN iSCSI in Windows, gli utenti devono connettersi alla LUN utilizzando iSCSI Software Initiator, lo strumento iSCSI proprietario di Microsoft. Per gli utenti che eseguono Windows Server 2008 o Windows Vista e versioni successive, iSCSI Software Initiator è integrato nel sistema operativo. Gli utenti che eseguono Windows Server 2003, Windows XP e Windows 2000 devono scaricare l'Initiator prima di completare questa procedura. Attieniti alla seguente procedura per connetterti a una LUN iSCSI in Windows con iSCSI Software Initiator.

## Stabilisci una connessione a una LUN iSCSI

1. Richiama **nome utente, password e indirizzo di archiviazione di iSCSI** per l'iSCSI in fase di connessione dal Portale del cliente. Fai riferimento alla schermata di accesso al trasferimento dati.
2. Avvia iSCSI Initiator.
3. Aggiorna il nome dell'Initiator nella scheda **Configurazione** nei dati IQN nel portale SoftLayer.
4. Fai clic sulla scheda **Individuazione**.
5. Fai clic sul pulsante **Aggiungi** nella sezione **Portali destinazione** della schermata.
6. Immetti l'**indirizzo IP iSCSI** nel campo **Indirizzo IP o nome DNS**.
7. Fai clic sulla scheda **Avanzate**.
8. Aggiorna le informazioni di accesso iSCSI.
   - Seleziona la casella di spunta **Informazioni di accesso CHAP** per abilitare l'accesso CHAP.
   - Immetti il **nome utente iSCSI** nel campo **Nome utente**.
   - Immetti la **password iSCSI** nel campo **Segreto destinazione**.
   - Fai clic sul pulsante **OK** due volte.
9. Fai clic sulla scheda **Destinazioni**.
10. Seleziona l'iSCSI appena aggiunta dall'elenco **Destinazioni**.
11. Fai clic sul pulsante **Accesso**. Verrà visualizzato il menu a comparsa **Accesso alla destinazione**.
12. Seleziona la casella di spunta **Ripristina automaticamente la connessione all'avvio del sistema** per impostare la connessione in modo che persista anche quando vengono eseguiti dei riavvii.
13. Fai clic sul pulsante **Avanzate**.
14. Aggiorna le informazioni di accesso iSCSI.
    - Seleziona la casella di spunta **Informazioni di accesso CHAP** per abilitare l'accesso CHAP.
    - Immetti il **nome utente iSCSI** nel campo **Nome utente**.
    - Immetti la **password iSCSI** nel campo **Segreto destinazione**.
    - Fai clic sul pulsante **OK** due volte.
15. Verifica che la nuova destinazione iSCSI venga visualizzata come Connessa nella scheda Destinazioni.

<table>
<tbody>
<tr>
<th>Se la destinazione iSCSI…</th><th>Allora...</th></tr>
<tr><td>Viene visualizzata come Connessa</td><td>Fai clic sul pulsante <strong>OK</strong>. La tua LUN iSCSI è ora connessa.</td></tr>
<tr><td>Non viene visualizzata come Connessa</td><td>Ripeti la procedura sopra indicata per reimpostare la connessione.</td></tr></tbody></table>
