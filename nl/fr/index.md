---

copyright:
  years: 1994, 2018
lastupdated: "2018-06-27"

---
{:new_window: target="_blank"}

# Initiation au service de transfert de données

Les utilisateurs peuvent employer le service de transfert de données {{site.data.keyword.BluSoftlayer_full}} pour envoyer un périphérique compatible USB 2.0 ou USB 3.0, des CD et des DVD à un centre de données {{site.data.keyword.BluSoftlayer}}. Leur périphérique est connecté directement à leur réseau, ce qui leur permet de contrôler à distance le transfert de données. Le périphérique est hébergé dans une armoire dédiée du centre de données client et est monté comme cible iSCSI. Le service de transfert de données constitue une solution idéale lorsque vous avez besoin de transférer de grandes quantités de données sans utiliser le réseau privé d'{{site.data.keyword.BluSoftlayer}}, et est offert gratuitement à tous les clients {{site.data.keyword.BluSoftlayer}}.

## Accès à l'écran Service de Transfert de Données

**Remarque** : cet écran est accessible uniquement à l'utilisateur principal du compte.

1. Accédez au portail [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} à l'aide de vos identifiants uniques.
2. Sélectionnez **Stockage** > **Migration de données** > **Transfert de Données** dans la barre de navigation pour accéder à l'écran du service de transfert de données. <br/>

Sur l'écran **Service de Transfert de données**, les utilisateurs peuvent soumettre une demande de transfert de données, afficher les détails concernant une demande, visualiser l'historique des tickets qui est associé au suivi du périphérique en vue d'effectuer une demande, et annuler une demande existante.

## Soumission d'une demande de transfert de données

Les demandes de transfert de données permettent au personnel approprié des centres de données d'être informé des expéditions client. Elles sont soumises via le portail [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. 

Lorsque vous créez une demande, gardez à l'esprit les instructions suivantes :

- Assurez-vous que le périphérique envoyé répond à toutes les [exigences matérielles](/docs/infrastructure/DataTransferService/data-transfer-service-faq.html).
- Vous ne pouvez associer qu'un seul périphérique à une demande. Si vous souhaitez envoyer plusieurs périphériques, vous devez créer une demande par périphérique.
- Si vous voulez récupérer le périphérique, fournissez une étiquette de retour prépayée, ainsi que les documents d'exportation nécessaires dans le colis afin que le périphérique vous soit restitué à l'issue du transfert.
- En cas d'expédition à l'international, il vous incombe d'effectuer toutes les démarches de licence, d'expédition et de dédouanement liées au périphérique. Vous devez notamment payer les frais de douane, les taxes et autres frais d'expédition pour faire parvenir le périphérique au centre de données {{site.data.keyword.BluSoftlayer}} et éventuellement le récupérer.
- Vous devez indiquer le nom du transporteur et le numéro de suivi de l'expédition vers le centre de données au moment de la demande.  Créez l'étiquette d'expédition en y apposant l'adresse de centre de données appropriée avant de soumettre la demande de transfert de données.

Suivez les étapes ci-après pour soumettre une demande de transfert de données.

1. Accédez à l'écran **Service de Transfert de Données** dans le portail [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}.
2. Cliquez sur **Commander demande de transfert de données**.
3. Renseignez chaque zone de la section **Informations sur l'unité** conformément au tableau 1.
<table border="1">
<caption>Le tableau 1 répertorie les noms des zones du formulaire de demande sur la gauche, et leur description sur la droite.</caption> 
 <tr><th>Nom de zone</th><th>Instructions</th></tr>
 <tr><td>Type de périphérique</td><td>Type de périphérique expédié. Si le type du périphérique ne figure pas dans la liste, sélectionnez "Autre".</td></tr>
 <tr><td>Numéro de série</td><td> Numéro de série du périphérique.</td></tr><tr><td>Description</td><td>Brève description du périphérique. Parmi les détails à mentionner, indiquez des facteurs permettant d'identifier le périphérique, tels que sa couleur, les étiquettes ou les stickers.</td></tr>
 <tr><td>Important</td><td>Toutes les remarques supplémentaires concernant le périphérique ou le transfert.</td></tr><tr><td>Destination</td><td>Centre de données chargé de recevoir le périphérique.</td></tr>
 <tr><td>Transporteur</td><td>Service postal ou express utilisé pour expédier le périphérique vers sa destination.</td></tr>
 <tr><td>Numéro de suivi</td><td>Numéro de suivi complet de l'envoi.</td></tr>
 </table>

4. Renseignez chaque zone de la section **Adresse de l'Expéditeur** ou cochez la case **Adresse de la société** pour compléter automatiquement les zones avec l'adresse de la société. <br/> **Remarque** : pensez à inclure l'étiquette de retour prépayée, ainsi que les documents d'exportation nécessaires dans le colis.
5. Après avoir pris connaissance du contrat de service, cochez la case **J'ai lu et j'accepte le Contrat de Service de Transfert de Données et le Contrat de Service de Référence**.
6. Cliquez sur **Soumettre Demande de Service**.

Une fois la demande soumise, le statut du ticket de demande apparaît comme `Envoyé à SoftLayer`. Veuillez nous informer si l'importation ou l'exportation nécessite une licence de la part de votre autorité locale, prévenez {{site.data.keyword.BluSoftlayer}} et joignez les informations de licence au ticket.

Dès réception du périphérique, le statut passe à `Reçu par SoftLayer`. Il passe ensuite à `Connecté` après qu'un technicien du centre de données a connecté le périphérique au réseau. 

Le délai de transfert de données initial est de deux semaines. Durant cette période, l'accès au périphérique est limité à l'administrateur du compte. Si vous avez besoin de plus de temps, demandez une prolongation. En outre, si vous souhaitez que le périphérique soit renvoyé en moins de deux semaines, vous pouvez demander le retour. Vous devez informer {{site.data.keyword.IBM}} par le biais du portail [{{site.data.keyword.slportal}}](https://control.softlayer.com/) lorsque le transfert est terminé. {{site.data.keyword.BluSoftlayer}} détache ensuite le périphérique et le renvoie ou le détruit, selon vos dispositions.


## Accès à l'écran Expéditions

L'écran Expéditions du portail [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} affiche l'ensemble des expéditions qui sont associées aux demandes du service de transfert de données. A partir de cet écran, vous pouvez afficher des expéditions et vous pouvez confirmer les expéditions des retours dès réception. 

Pour accéder à l'écran Expéditions :

1. Accédez au portail [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} à l'aide de vos identifiants uniques.
2. Sélectionnez **Compte** > **Gérer** > **Expéditions** dans la barre de navigation.

Sur l'écran Expéditions, toutes les demandes d'expédition des 30 derniers jours sont affichées, avec les informations détaillées les concernant. Vous pouvez appliquer une fonction de [tri ou de filtre](sort-or-filter-shipments-list.html) par statut, âge ou détails spécifiques d'expédition. De plus, vous pouvez confirmer la réception d'un retour depuis cet écran.
![Ecran Expéditions](/images/DTSShipmentScreen1.png)
