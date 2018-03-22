---

copyright:
  years: 2017
lastupdated: "2017-11-13"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}

# Connexion à l'unité DTS sous Linux pour CentOS/RHEL 7

Pour interagir avec un numéro d'unité logique iSCSI dans des systèmes d'exploitation de type Linux, les utilisateurs se connectent au numéro d'unité logique en saisissant une série de commandes dans le terminal basé sur le système d'exploitation utilisé pour l'exécution des interactions. L'outil utilisé pour interagir avec un numéro d'unité logique iSCSI dans un système d'exploitation de type Linux dépend du type et de la version du système d'exploitation installé sur le terminal.

## Instructions pour CentOS 7 et RHEL 7

1. Installez iscsi-initiator et le module de mappage multi-accès pour Linux <br/>
   ``   yum -y install iscsi-initiator-utils device-mapper device-mapper-multipath
   `` 
2. Créez le fichier de configuration iscsid.conf <br/>
3. Sauvegardez la configuration d'origine : <br/>
   ``   cp /etc/iscsi/iscsid.conf{,.save}
   `` 
4. Ouvrez le fichier /etc/iscsi/iscsid.conf dans votre éditeur de texte favori et remplacez son contenu par : <br/>
   ``node.startup = automatic ``<br/>
   ``node.session.auth.username = ISCSI_USER ``<br/>
   ``node.session.auth.password = ISCSI_PASS ``<br/>
   ``discovery.sendtargets.auth.username = ISCSI_USER ``<br/>
   ``discovery.sendtargets.auth.password = ISCSI_PASS ``<br/>
   ``node.session.timeo.replacement_timeout = 120 ``<br/>
   ``node.conn[0].timeo.login_timeout = 15 ``<br/>
   ``node.conn[0].timeo.logout_timeout = 15 ``<br/>
   ``node.conn[0].timeo.noop_out_interval = 10 ``<br/>
   ``node.conn[0].timeo.noop_out_timeout = 15 ``<br/>
   ``node.session.iscsi.InitialR2T = No ``<br/>
   ``node.session.iscsi.ImmediateData = Yes ``<br/>
   ``node.session.iscsi.FirstBurstLength = 262144 ``<br/>
   ``node.session.iscsi.MaxBurstLength = 16776192 ``<br/>
   ``node.conn[0].iscsi.MaxRecvDataSegmentLength = 65536 ``<br/>
5. Démarrez iscsid :<br/>
   ``    /etc/init.d/iscsi start
   ``
6. Lancez une  reconnaissance sur l'hôte cible iscsi :<br/>
   ``   iscsiadm -m discovery -t sendtargets -p [IP Address in StorageLayer]
   ``
7. Connectez-vous à l'hôte cible iscsi :<br/>
   ``   iscsiadm -m node -T [output from above starting with iqn.] -p [IP Address in storagelayer] -l
   ``
8. Redémarrez le service iscsi (la connexion est établie automatiquement à l'hôte cible, car node.startup a la valeur automatic dans iscsid.conf).<br/>
   ``    /etc/init.d/iscsi restart
   ``
