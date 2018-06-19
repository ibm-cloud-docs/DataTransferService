---

copyright:
  years: 2017, 2018
lastupdated: "2018-05-22"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Qu'est-ce qu'un service de transfert de données ?
 
Le service de transfert de données vous permet d'envoyer un périphérique compatible USB 2.0 ou 3.0, des CD et des DVD vers un centre de données {{site.data.keyword.BluSoftlayer_full}} afin de les connecter directement à votre réseau. Le périphérique est hébergé dans une armoire dédiée et est monté comme cible iSCSI. Les disques Advanced Format (AF) sont désormais pris en charge.

## Exigences liées au matériel
1.    L'alimentation électrique du périphérique doit être compatible 208v/220v
2.    La fiche secteur du périphérique doit être compatible avec un connecteur 120v standard (NEMA 5-15P)
3.    Le périphérique doit être compatible USB 2.0 (3.0 est également pris en charge maintenant)
4.    Le périphérique doit être équipé d'un câble USB avec un connecteur mâle USB (prise standard installée sur la plupart des ordinateurs)
5.    CD/DVD
      1.    Les supports doivent être rangés dans des boîtes, boîtiers ou tout autre conteneur prévus à cet effet et ils doivent être de préférence stockés tous ensemble dans un même conteneur (boîte de CD, par exemple), chaque disque étant soigneusement étiqueté de manière unique.
      2.    Les disques seront enchaînés à la demande du client via le ticket

## Frais à votre charge
1.    Demande initiale de service : $0
2.    Premières deux semaines de transfert de données : $0
      **Remarque** : $25 seront ensuite facturés par semaine d'extension
3.    Les coûts d'expédition aller-retour depuis le centre de données {{site.data.keyword.IBM}}, incluant tous les frais et taxes.

**Remarque **: Le client est responsable des points suivants :  
- Vous devez vous assurer qu'aucune licence d'importation ou d'exportation n'est requise pour expédier le périphérique vers le centre de données {{site.data.keyword.IBM}} ou pour le renvoyer au client (le cas échéant). 
- Vous devez vous assurer que ni le client ni un utilisateur du client dont les données sont incluses ne sont soumis à une ordonnance du gouvernement américain leur refusant ou leur révoquant leurs droits d'exportation. Avertissez immédiatement {{site.data.keyword.IBM}} si le client ou un tel utilisateur final devient soumis à ce type d'ordonnance.  
- Vous devez effectuer toutes les démarches de licence, d'expédition et de dédouanement liées au périphérique. Il incombe au client de notamment payer les frais de douane, les taxes et autres frais d'expédition pour faire parvenir le périphérique au centre de données {{site.data.keyword.IBM}} et éventuellement le récupérer.    
- Vous devez observer toutes les lois applicables en ce qui concerne l'expédition et le retour du périphérique et le transfert du contenu vers le centre de données {{site.data.keyword.IBM}}.Cela inclut les lois en matière de confidentialité, d'importation et d'exportation. 
- Vous devez avoir mis en place des accords appropriés, et obtenu tous les droits nécessaires, avec l'utilisateur du client en ce qui concerne le transfert matériel des données de l'utilisateur par le client.

## Processus de demande
Vous effectuez une demande en cliquant sur **Stockage** > **Migration de données** >  **Transfert de données**, puis en cliquant sur **Commander Demande de Transfert de Données** dans l'angle supérieur droit. 

![Demande de transfert de données](/images/DTS.png)

Renseignez le formulaire en indiquant les informations suivantes relatives au périphérique :
1. Numéro de série
2. Type
3. Brève description du périphérique
4. Centre de données vers lequel expédier le périphérique
5. Numéro de suivi permettant de suivre l'expédition
6. Service de transport utilisé
7. Adresse de retour à laquelle renvoyer le périphérique une fois le transfert terminé

Cette demande crée un ticket de demande d'assistance afin de prévenir nos techniciens de l'arrivée prochaine du périphérique et de leur permettre de suivre l'expédition. Une fois le périphérique reçu, nous le connecterons à votre armoire dédiée. Une fois le périphérique connecté, le ticket est mis à jour afin de vous fournir un lien vers vos données d'identification de connexion à la cible iSCSI.

## Demande de retour
Si vous avez fourni une adresse de retour et inclut l'étiquette de retour prépayée dans le colis, vous pouvez demander que le périphérique vous soit renvoyé n'importe quand pendant le délai des deux semaines du transfert. Pour cela, utilisez le portail [{{site.data.keyword.slportal}}](https://control.softlayer.com/){:new_window}. Sélectionnez **Stockage** > **Migration de données** > **Transfert de données** et dans le menu **Action** de votre périphérique, sélectionnez **Demande de retour**. Un message est alors envoyé à nos techniciens afin de les informer qu'ils doivent déconnecter le périphérique et vous le renvoyer.

## Demande d'extension
Une fois la période de deux semaines gratuites écoulée, si vous avez encore besoin d'utiliser votre périphérique, vous devez faire une demande d'extension. Vous préviendrez ainsi nos techniciens de l'extension de la durée de connexion du périphérique. Pour ce faire, vous pouvez procéder comme pour une demande de retour de périphérique. Sélectionnez **Stockage** > **Migration de données** > **Transfert de données** et dans le menu **Action** de votre périphérique, sélectionnez **Extension de demande**. Chaque semaine supplémentaire induit des frais de service obligatoires d'un montant de $25. Notez que votre demande d'extension est susceptible d'être refusée selon l'espace disponible dans le centre de données. Lorsque la demande est acceptée, le ticket est mis à jour en conséquence. 

## Déconnexion
Au terme de la période de deux semaines, le périphérique est automatiquement déconnecté de notre centre de données. Si vous avez demandé un retour, votre périphérique vous est renvoyé par le transporteur de votre choix et à l'adresse de retour que vous avez spécifiée dans la demande initiale. Le ticket est mis à jour pour stipuler que le périphérique a été déconnecté. Si vous n'avez pas demandé le retour du périphérique, celui-ci est détruit sur site.
