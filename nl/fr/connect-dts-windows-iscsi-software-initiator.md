---

copyright:
  years: 2017
lastupdated: "2017-11-13"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Connexion à l'unité DTS sous Windows via l'initiateur logiciel iSCSI 

Pour interagir avec un numéro d'unité logique iSCSI sous Windows, les utilisateurs se connectent au numéro d'unité logique à l'aide de l'initiateur logiciel iSCSI, l'outil iSCSI propriétaire de Microsoft. Pour les utilisateurs exécutant Windows Server 2008 ou Windows Vista et versions ultérieures, l'initiateur logiciel iSCSI est intégré au système d'exploitation. Les utilisateurs exécutant Windows Server 2003, Windows XP et Windows 2000 doivent quant à eux télécharger le logiciel avant de réaliser la procédure ci-dessous. Suivez les étapes ci-dessous pour vous connecter à un numéro d'unité logique dans Windows via l'initiateur logiciel iSCSI.

## Connexion à un numéro d'unité logique iSCSI

1. Récupérez les **nom d'utilisateur, mot de passe et adresse mémoire iSCSI** correspondant à l'interface iSCSI actuellement connectée dans le portail client. Voir la rubrique Accéder à l'écran Transfert de données.
2. Lancez l'initiateur iSCSI.
3. Mettez à jour le nom de l'initiateur dans l'onglet **Configuration** avec les données IQN du portail SoftLayer.
4. Cliquez sur l'onglet **Reconnaissance**.
5. Cliquez sur le bouton **Ajouter** dans la section **Portails cibles** de l'écran.
6. Entrez l'**adresse IP iSCSI** dans la zone **Adresse IP ou Nom DNS**.
7. Cliquez sur l'onglet **Avancé**.
8. Mettez à jour les informations de connexion iSCSI.
   - Sélectionnez la case relative aux **informations de connexion CHAP** pour activer la connexion correspondante.
   - Entrez le **nom d'utilisateur iSCSI** dans la zone **Nom d'utilisateur**.
   - Entrez le **mot de passe iSCSI** dans la zone relative à la **valeur confidentielle de la cible**.
   - Cliquez à deux reprises sur le bouton **OK**.
9. Cliquez sur l'onglet **Cibles**.
10. Sélectionnez la dernière interface iSCSI ajoutée à partir de la liste **Cibles**.
11. Cliquez sur le bouton **Connexion**. Le menu contextuel de **connexion à la cible** s'affiche.
12. Cochez la case permettant de **restaurer automatiquement la connexion au démarrage du système** afin de maintenir la connexion entre chaque lancement.
13. Cliquez sur le bouton **Avancé**.
14. Mettez à jour les informations de connexion iSCSI.
    - Sélectionnez la case relative aux **informations de connexion CHAP** pour activer la connexion correspondante.
    - Entrez le **nom d'utilisateur iSCSI** dans la zone **Nom d'utilisateur**.
    - Entrez le **mot de passe iSCSI** dans la zone relative à la **valeur confidentielle de la cible**.
    - Cliquez à deux reprises sur le bouton **OK**.
15. Vérifiez que la nouvelle cible iSCSI apparaît comme Connectée dans l'onglet Cibles.

<table>
<tbody>
<tr>
<th>Si la cible iSCSI…</th><th>Alors...</th></tr>
<tr><td>S'affiche avec l'état Connecté</td><td>Cliquez sur le bouton <strong>OK</strong>. Votre numéro d'unité logique iSCSI est maintenant connecté. </td></tr>
<tr><td>Ne s'affiche pas avec l'état Connecté</td><td>Répétez les étapes ci-dessus pour réinitialiser la connexion.</td></tr></tbody></table>
