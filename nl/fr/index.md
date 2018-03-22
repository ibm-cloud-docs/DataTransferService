---

copyright:
  years: 1994, 2017
lastupdated: "2017-12-18"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Initiation au service de transfert de données

Le service de transfert de données {{site.data.keyword.BluSoftlayer_full}} permet aux clients d'envoyer une unité compatible USB 2.0 ou USB 3.0 et/ou des CD et DVD à un centre de données {{site.data.keyword.BluSoftlayer}} afin de les connecter directement à leur réseau et contrôler à distance le transfert de données. L'unité est hébergée dans une armoire dédiée du centre de données client et est montée comme cible iSCSI. Notre service de transfert de données constitue une solution idéale lorsque vous avez besoin de transférer de gros volumes de données sans utiliser notre réseau privé, et est offert gratuitement à tous les clients {{site.data.keyword.BluSoftlayer}}.

## Accès à l'écran Service de Transfert de Données

**Remarque **: Cet écran est pour l'instant accessible uniquement à l'utilisateur principal du compte.

1. Accédez au portail [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} à l'aide de vos identifiants uniques.
2. Sélectionnez **Stockage** > **Migration de données** > **Transfert de Données** dans la barre de navigation pour accéder à l'écran du service de transfert de données. <br/>

L'écran Service de Transfert de Données s'ouvre, à partir duquel les utilisateurs ont la possibilité de soumettre une demande de transfert de données, d'afficher les détails concernant une demande, de visualiser l'historique des tickets associés au suivi de l'unité en vue d'effectuer une demande, et d'annuler une demande existante.

## Demande de transfert de données

Les demandes de transfert de données permettent au personnel approprié des centres de données d'être informé des expéditions client. Elles sont soumises via le portail [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. Lorsque vous créez une demande, gardez à l'esprit les instructions suivantes :

- Assurez-vous que l'unité envoyée avec la demande satisfait toutes les [exigences matérielles](/docs/infrastructure/DataTransferService/data-transfer-service-faq.html).
- Vous ne pouvez associer qu'une seule unité par demande. Si vous souhaitez envoyer plusieurs unités, vous devez créer une demande par unité.
- Si vous voulez récupérer l'unité, fournissez une étiquette de retour prépayée ainsi que les documents d'exportation nécessaires dans le colis afin que l'unité vous soit restituée à l'issue du transfert.
- En cas d'expédition internationale, il vous incombe d'effectuer toutes les démarches de licence, d'expédition et de dédouanement liées à l'unité, y compris le paiement des frais de douane, taxes et autres frais d'expédition pour faire parvenir l'unité au centre de données IBM et éventuellement la récupérer.
- Le transporteur et le numéro de suivi de l'expédition vers notre centre de données doivent être indiqués au moment de la demande. Vérifiez que l'étiquette a été créée avec la bonne adresse de centre de données avant de terminer la demande.

Suivez les étapes ci-dessous pour soumettre une demande de transfert de données.

1. Accédez à l'écran **Service de Transfert de Données** dans le portail [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. <br/> **Remarque **: Cet écran est accessible uniquement à l'utilisateur principal du compte.
2. Cliquez sur **Commander Demande de Transfert de Données** en haut de l'écran.
3. Renseignez chaque zone de la section **Informations sur l'Unité** conformément au tableau ci-dessous. 
<table border="1">
<tbody>
 <tr><th>Nom de zone</th><th>Instructions</th></tr>
 <tr><td>Type d'unité</td><td>Type d'unité à expédier. Si le type de l'unité ne figure pas dans la liste, sélectionnez "Autre".</td></tr>
 <tr><td>Numéro de série</td><td> Numéro de série de l'unité.</td></tr><tr><td>Description</td><td>Brève description de l'unité. Parmi les détails à mentionner, indiquez des facteurs permettant d'identifier l'unité, tels que sa couleur, les étiquettes ou stickers apposés dessus, etc.</td></tr>
 <tr><td>Important</td><td>Toutes remarques supplémentaires concernant l'unité ou le transfert.</td></tr><tr><td>Destination</td><td>Le centre de données chargé de recevoir l'unité.</td></tr>
 <tr><td>Transporteur</td><td>Service postal ou express utilisé pour expédier l'unité vers sa destination.</td></tr>
 <tr><td>Numéro de suivi</td><td>Numéro de suivi complet de l'envoi.</td></tr>
 </tbody>
 </table>

4. Renseignez chaque zone de la section **Adresse de l'Expéditeur** ou cochez la case **Adresse de la société** pour compléter automatiquement les zones avec l'adresse de la société. <br/> **Remarque **: Pensez à inclure l'étiquette de retour prépayée ainsi que les documents d'exportation nécessaires dans le colis afin que l'unité vous soit renvoyée à l'issue du transfert.
5. Cochez la case **J'ai lu et j'accepte le Contrat de Service de Transfert de Données et le Contrat de Service de Référence** après avoir pris connaissance des contrats.
6. Cliquez sur **Soumettre Demande de Service** pour envoyer la demande. Cliquez sur **Annuler** pour annuler l'action.

Une fois la demande soumise, le statut du ticket apparaît comme *Envoyé à SoftLayer*. Veuillez nous informer si l'importation ou l'exportation nécessite une licence de la part de votre autorité locale et joignez les informations de licence au ticket.

Dès réception de l'unité, le statut est mis à jour en *Reçu par SoftLayer*, puis en *Connecté* lorsqu'un technicien du centre de données a connecté l'unité à notre réseau. 

Le délai de transfert de données initial est de deux (2) semaines maximum. Durant cette période, l'accès à l'unité est limité à l'administrateur du compte. Si un délai supplémentaire est requis, une demande d'extension doit être effectuée. Inversement, si l'unité doit être livrée avant le délai des deux (2) semaines, une demande de retour doit être effectuée. Informez {{site.data.keyword.IBM}} par le biais du portail [{{site.data.keyword.slportal}}](https://control.softlayer.com/) une fois le transfert terminé. Nous détacherons alors l'unité et celle-ci sera soit réexpédiée ou détruite, selon vos dispositions.


## Accès à l'écran Expéditions

L'écran Expéditions du portail [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} affiche l'ensemble des expéditions associées aux demandes du service de transfert de données. Dans cet écran, vous pouvez visualiser les expéditions et confirmer les retours après réception. Suivez les étapes ci-dessous pour accéder à l'écran Expéditions.

1. Accédez au portail [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} à l'aide de vos identifiants uniques.
2. Sélectionnez **Compte** > **Gérer** > **Expéditions** dans la barre de navigation pour accéder à l'écran Expéditions.

Lorsque vous accédez à l'écran Expéditions, les demandes d'expédition des 30 derniers jours sont affichées dans la liste des expéditions avec le détail de chaque expédition. Vous pouvez appliquer une fonction de [tri ou de filtre](sort-or-filter-shipments-list.html) par statut, âge ou détails spécifiques d'expédition. De plus, vous pouvez confirmer la réception d'un retour depuis cet écran.
![Ecran Expéditions](/images/DTSShipmentScreen1.png)
