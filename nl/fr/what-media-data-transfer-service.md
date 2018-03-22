---

copyright:
  years: 2017
lastupdated: "2017-12-18"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Qu'est que le service de transfert de données sur support ?
 
Le service de transfert de données est un service qui vous permet d'envoyer une unité compatible USB 2.0 ou 3.0 et/ou des CD et DVD vers un centre de données {{site.data.keyword.BluSoftlayer_full}} afin de les connecter directement à votre réseau. L'unité est hébergée dans une armoire dédiée du centre de données de votre choix et est montée en tant que cible iSCSI. Les disques Advanced Format (AF) sont désormais pris en charge.

## Exigences liées au matériel
1.    L'alimentation électrique de l'unité doit être compatible 208v/220v
2.    La fiche secteur de l'unité doit être compatible avec un connecteur 120v standard (NEMA 5-15P)
3.    L'unité doit être compatible USB 2.0 (3.0 est également pris en charge maintenant)
4.    L'unité doit être équipée d'un câble USB avec un connecteur mâle USB (prise standard installée sur la plupart des ordinateurs)
5.    CD/DVD
      1.    Les supports doivent être rangés dans des boîtes, boîtiers ou tout autre conteneur prévus à cet effet et ils doivent être de préférence stockés tous ensemble dans un même conteneur (boîte de CD, par exemple), chaque disque étant soigneusement étiqueté de manière unique.
      2.    Les disques seront enchaînés à la demande du client via le ticket

## Frais à votre charge
1.    Demande initiale de service : $0
2.    Premières deux semaines de transfert de données : $0
      **Remarque** : $25 seront ensuite facturés par semaine d'extension
3.    Les coûts d'expédition aller-retour depuis le centre de données {{site.data.keyword.IBM}}, incluant tous les frais et taxes.

**Remarque **: Le client est responsable des points suivants :  
- Vous devez vous assurer qu'aucune licence d'importation ou d'exportation n'est requise pour expédier l'unité vers le centre de données {{site.data.keyword.IBM}} ou pour la renvoyer au client (le cas échéant).  
- Vous devez vous assurer que ni le client ni un utilisateur final du client dont les données sont incluses ne sont soumis à une ordonnance du gouvernement américain leur refusant ou révoquant leurs droits d'exportation. Le client s'engage à avertir immédiatement {{site.data.keyword.IBM}} si le client ou un tel utilisateur final devient soumis à ce type d'ordonnance.  
- Vous devez effectuer toutes les démarches de licence, d'expédition et de dédouanement liées à l'unité, y compris le paiement des frais de douane, taxes et autres frais d'expédition pour faire parvenir l'unité au centre de données {{site.data.keyword.IBM}} et éventuellement l'en faire revenir.   
- Vous devez observer toutes les lois applicables, notamment en matière de protection des données, d'importation et d'exportation, en ce qui concerne l'expédition et le retour de l'unité et le transfert du contenu vers le centre de données {{site.data.keyword.IBM}}. 
- Vous devez avoir mis en place des accords appropriés, et obtenu tous les droits nécessaires, avec l'utilisateur final du client en ce qui concerne le transfert matériel des données de l'utilisateur final par le client.

## Processus de demande
Vous effectuez une demande en cliquant sur **Stockage** > **Migration de données** >  **Transfert de données**, puis en cliquant sur le lien **Commander Demande de Transfert de Données** situé en haut à droite de la page.

![Demande de transfert de données](/images/DTS.png)
 

Remplissez le formulaire associé aux unités
1. Numéro de série
2. Type
3. Brève description de l'unité
4. Centre de données vers lequel expédier l'unité
5. Numéro de suivi permettant de suivre la livraison
6. Service de transport utilisé
7. Adresse de retour à laquelle renvoyer l'unité une fois le transfert terminé

Une fois ces renseignements fournis, un ticket de demande d'assistance est automatiquement créé afin de prévenir nos techniciens de l'arrivée prochaine de l'unité et de leur permettre de suivre la livraison. Une fois l'unité reçue, nous la connecterons à votre armoire dédiée. Lorsque l'unité est connectée, le ticket est mis à jour et vous indique le lien à suivre pour vous connecter à votre cible iSCSI à l'aide de vos identifiants.

## Demande de retour
Si vous avez fourni une adresse de retour et inclut l'étiquette de retour prépayée dans le colis, vous pouvez demander à ce que l'unité vous soit renvoyée n'importe quand pendant le délai des deux semaines du transfert. Pour ce faire, accédez au portail [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window} en cliquant sur **Stockage** > **Migration de données** > **Transfert de données**, puis en sélectionnant l'option **Demande de retour** dans la liste déroulante **Action** de votre unité. Un message est alors envoyé à nos techniciens afin de les informer qu'ils doivent déconnecter l'unité et vous la renvoyer.

## Demande d'extension
Une fois la période de deux semaines gratuites écoulée, si vous avez encore besoin d'utiliser votre unité USB, faites une demande d'extension afin de prévenir nos techniciens de l'extension de la  durée de connexion de l'unité. Pour ce faire, procédez comme si vous vouliez demander le retour de votre unité en cliquant sur **Stockage** > **Migration de données** > **Transfert de données**, puis en sélectionnant **Demande d'extension** dans la liste déroulante **Action** de l'unité. Chaque semaine supplémentaire vous coûtera 25 dollars. En outre, votre demande peut se voir refuser en fonction de l'espace disponible dans le centre de données. Si la demande est acceptée, le ticket est mis à jour afin de refléter l'extension d'une semaine supplémentaire.

## Déconnexion 
Une fois la période des deux semaines écoulée, l'unité est automatiquement déconnectée de notre centre de données et vous est renvoyée via le transporteur de votre choix et à l'adresse de retour que vous avez spécifiée dans votre demande d'origine. Le ticket est alors mis à jour afin d'indiquer que l'unité a été déconnectée. Si vous n'avez pas demandé le retour de l'unité, celle-ci sera détruite sur site.
