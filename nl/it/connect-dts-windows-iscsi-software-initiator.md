---

copyright:
  years: 2017, 2018
lastupdated: "2018-05-22"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Connessione a un dispositivo DTS in Windows con iSCSI Software Initiator

Per interagire con una LUN iSCSI in Windows, gli utenti devono connettersi all'archiviazione utilizzando iSCSI Software Initiator, lo strumento iSCSI proprietario di Microsoft. Per gli utenti di Windows Server 2008 o Windows Vista e versioni successive, iSCSI Software Initiator è integrato nel sistema operativo. Gli utenti di Windows Server 2003, Windows XP e Windows 2000 devono scaricare l'Initiator prima di avviare questa procedura.

## Stabilisci una connessione a una LUN iSCSI

1. Dal {{site.data.keyword.slportal}}, richiama **nome utente, password e indirizzo di archiviazione di iSCSI** dal dispositivo di archiviazione per cui vuoi stabilire la connessione.
2. Avvia iSCSI Initiator.
3. Nella scheda **Configuration**, aggiorna il nome dell'Initiator nei dati IQN nel {{site.data.keyword.slportal}}.
4. Fai clic su **Discovery**.
5. Nella sezione **Target Portals**, fai clic su **Add**.
6. Nel campo **IP address or DNS name**, immetti l''**indirizzo IP iSCSI**.
7. Fai clic su **Advanced**.
8. Aggiorna le informazioni di accesso iSCSI.
   - Seleziona la casella di spunta **CHAP logon information** per abilitare l'accesso CHAP.
   - Immetti il nome utente iSCSI nel campo **user name**.
   - Immetti la password nel campo **target secret**.
   - Fai clic su **OK** due volte.
9. Fai clic su **Targets**
10. Seleziona l'iSCSI appena aggiunta dall'elenco **Targets**.
11. Fai clic su **Logon**. Viene visualizzata la finestra **Log On to Target**.
12. Seleziona la casella di spunta **Automatically restore this connection when the system boots** e impostare la connessione in modo che persista anche quando vengono eseguiti dei riavvii.
13. Fai clic su **Advanced**.
14. Aggiorna le informazioni di accesso iSCSI.
    - Seleziona la casella di spunta **CHAP logon information** per abilitare l'accesso CHAP.
    - Immetti il nome utente iSCSI nel campo **user name**.
    - Immetti la password nel campo **target secret**.
    - Fai clic su **OK** due volte.
15. Verifica che la nuova destinazione iSCSI venga visualizzata come Connected nella scheda Targets.
    - Se la tua destinazione iSCSI viene visualizzata come **Connected**, fai clic su **OK**. La tua LUN iSCSI è ora connessa.
    - Se la tua destinazione iSCSI non viene visualizzata come **Connected**, ripeti tutta la procedura precedente per reimpostare la connessione.
