# TP_JONAS_DEVNET
Ce travail consiste à se connecter aux routeurs cisco sur le sandbox de developper.cisco.com, afin d'exécuter quelques commandes d'affichage (Show), récuperer le résultat et faire le traitement.
concrétement, le travail consiste à se connecter aux routeurs cisco via SSH, afficher le résumé des interfaces et la table de routage; puis afficher :
  -le nombre d'interfaces activées
  -le nombre d'interface désactivées
  -la liste des réseaux connectés directements au routeurs. 
  -NB. S'agissant des réseaux connectés directement, toute route configurée avec comme paramètre , l'interface de sortie, va apparaitre dans la liste comme réseau connecté directement.
  Pour réaliser ce lab, deux fichiers nous sont utiles: le fichier hosts dans lequel nous definissons les routeurs et leurs paramètres de connexion via SSH; ainsi que le playbook pour écrire notre code afin d'exécuter 
  toutes les tâches.
  Après avoir créer le fichier hosts, vous pouvez essayer de faire ping vers les routeurs en exécutant la commande: ansible routers -m ping.
  et vous pouvez vous rassurer que tout va bien en exécutant à partir du terminal linux la commande suivant: ansible routers -m ios_command -a "commands='show ip int brief' .

Si le routeur présent dans le fichier hosts n'est pas accessible, utilisez celui-ci: ios-xe-mgmt.cisco.com avec les mêmes identifiants de connexion.

