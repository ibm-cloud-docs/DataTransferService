---

copyright:
  years: 2017, 2018
lastupdated: "2018-06-27"

---
{:new_window: target="_blank"}

# Connexion au périphérique DTS sous Windows via l'initiateur logiciel iSCSI

Pour interagir avec un numéro d'unité logique iSCSI sous Windows, les utilisateurs doivent se connecter à la mémoire à l'aide de l'initiateur logiciel iSCSI, l'outil iSCSI propriétaire de Microsoft. Pour les utilisateurs de Windows Server 2008, Windows Vista ou des versions ultérieures, l'initiateur logiciel iSCSI est intégré au système d'exploitation. Les utilisateurs de Windows Server 2003, Windows XP et Windows 2000 doivent télécharger l'initiateur avant de commencer la procédure ci-dessous.

## Connexion à un numéro d'unité logique iSCSI

1. Sur le portail {{site.data.keyword.slportal}}, récupérez les **nom d'utilisateur, mot de passe et adresse mémoire iSCSI** correspondant au périphérique de stockage à connecter.
2. Démarrez l'initiateur iSCSI.
3. Sur l'onglet **Configuration**, mettez à jour le nom de l'initiateur avec le nom qualifié iSCSI du portail {{site.data.keyword.slportal}}.
4. Cliquez sur **Discovery**.
5. Dans la section **Target Portals**, cliquez sur **Add**.
6. Dans la zone **IP address or DNS name**, entrez l'**adresse IP iSCSI**.
7. Cliquez sur **Advanced**.
8. Mettez à jour les informations de connexion iSCSI.
   - Sélectionnez la case relative aux **informations de connexion CHAP** pour activer la connexion correspondante.
   - Entrez le nom d'utilisateur iSCSI dans la zone **user name**.
   - Entrez le mot de passe iSCSI dans la zone **target secret**.
   - Cliquez deux fois sur **OK**.
9. Cliquez sur **Targets**
10. Sélectionnez la dernière interface iSCSI ajoutée à partir de la liste **Targets**.
11. Cliquez sur **Logon**. La fenêtre **Log On to Target** s'affiche.
12. Sélectionnez **Automatically restore this connection when the system boots** afin de maintenir la connexion entre chaque redémarrage.
13. Cliquez sur **Advanced**.
14. Mettez à jour les informations de connexion iSCSI.
    - Sélectionnez la case relative aux **informations de connexion CHAP** pour activer la connexion correspondante.
    - Entrez le nom d'utilisateur iSCSI dans la zone **user name**.
    - Entrez le mot de passe iSCSI dans la zone **target secret**.
    - Cliquez deux fois sur **OK**.
15. Vérifiez que la nouvelle cible iSCSI apparaît avec l'état Connected sur l'onglet Targets.
    - Si votre cible iSCSI a pour état **Connected**, cliquez sur **OK**. Votre numéro d'unité logique iSCSI est désormais connecté.
    - Si votre cible iSCSI n'est pas à l'état**Connected**, répétez toutes les étapes précédentes pour réinitialiser la connexion.
