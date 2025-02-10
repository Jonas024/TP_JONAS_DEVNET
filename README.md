# TP_JONAS_DEVNET
Ce travail consiste à se connecter aux routeurs cisco sur le sandbox de developper.cisco.com, afin d'exécuter quelques commandes d'affichage (Show), récuperer le résultat et faire le traitement.
concrétement, le travail consiste à se connecter aux routeurs cisco via SSH, afficher le résumé des interfaces et la table de routage; puis afficher :
  le nombre d'interfaces activées
  le nombre d'interface désactivées
  la liste des réseaux connectés directements au routeurs. 
  NB. S'agissant des réseaux connectés directement, toute route configyrée avec comme paramètre , l'interface de sortie, va apparaitre dans la liste comme route connecté directement.
  Pour réaliser ce lab, deux fichiers nous sont utiles: le fichier hosts dans lequel nous definissons les routeurs et leurs paramètres de connexion via SSH; ainsi que le playbook pour écrire notre code afin d'exécuter 
  toutes les tâches.
  
