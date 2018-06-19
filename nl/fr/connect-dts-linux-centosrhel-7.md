---

copyright:
  years: 2017, 2018
lastupdated: "2017-05-22"

---
{:pre: .pre}

# Connexion au périphérique DTS sous Linux pour CentOS/RHEL 7

Pour interagir avec un numéro d'unité logique iSCSI dans des systèmes d'exploitation de type Linux, les utilisateurs se connectent au numéro d'unité logique en saisissant une série de commandes dans le terminal. L'outil utilisé pour interagir avec un numéro d'unité logique iSCSI dans un système d'exploitation de type Linux dépend du type et de la version du système d'exploitation qui est installé sur le terminal.

## Instructions pour CentOS 7 et RHEL 7

1. Installez iscsi-initiator et le mappeur multi-accès pour Linux.
   ```
   yum -y install iscsi-initiator-utils device-mapper device-mapper-multipath
   ``` 
   {: pre}
   
2. Créez le fichier de configuration iscsid.conf.

3. Sauvegardez la configuration d'origine : 
   ```
   cp /etc/iscsi/iscsid.conf{,.save}
   ``` 
   {: pre}
   
4. Ouvrez le fichier /etc/iscsi/iscsid.conf dans votre éditeur de texte favori et remplacez son contenu par le code suivant :  
   ```
   node.startup = automatic
   node.session.auth.username = ISCSI_USER
   node.session.auth.password = ISCSI_PASS
   discovery.sendtargets.auth.username = ISCSI_USER
   discovery.sendtargets.auth.password = ISCSI_PASS
   node.session.timeo.replacement_timeout = 120
   node.conn[0].timeo.login_timeout = 15
   node.conn[0].timeo.logout_timeout = 15
   node.conn[0].timeo.noop_out_interval = 10
   node.conn[0].timeo.noop_out_timeout = 15
   node.session.iscsi.InitialR2T = No
   node.session.iscsi.ImmediateData = Yes
   node.session.iscsi.FirstBurstLength = 262144
   node.session.iscsi.MaxBurstLength = 16776192
   node.conn[0].iscsi.MaxRecvDataSegmentLength = 65536
   ```
   {: pre}

5. Démarrez iscsi :<br/>
   ```
   /etc/init.d/iscsi start
   ```
   {: pre}
   
6. Lancez une  reconnaissance sur l'hôte cible iscsi :<br/>
   ```
   iscsiadm -m discovery -t sendtargets -p [IP address in StorageLayer]
   ```
   {: pre}
   
7. Connectez-vous à l'hôte cible iscsi :<br/>
   ```
   iscsiadm -m node -T [output from previous command, starting with IQN.] -p [IP address in StorageLayer] -l
   ```
   {: pre}
   
8. Redémarrez le service iscsi (la connexion est établie automatiquement à l'hôte cible, car la valeur automatic est affectée à node.startup dans iscsid.conf).<br/>
   ```
   /etc/init.d/iscsi restart
   ```
   {: pre}
