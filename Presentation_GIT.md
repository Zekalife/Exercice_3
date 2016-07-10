#<p style="text-align:center;"> Présentation de GIT

## GIT 
<div style="text-align:justify;">
GIT est un logiciel de gestion de version basé sur le modèle distribué. Développé par Linus Torvalds, l'auteur de Linux, il est l'un des plus utilisé actuellement et connais un succès grandissant. Le code peut être partagé directement entre deux développeur mais peut également être installé sur le site [GITHUB](http://github.com). Ce site héberge plusieurs millions de projet opensource pour la plupart. Il est toutefois possible d'ouvrir un compte payant pour y créer des dépôts (repository en anglais) privés.

Rentrons maintenant dans le fonctionnement de GIT

### Commit
Au fur et à mesure de la rédaction du code et la création des fichiers, il est nécessaire de créer des points étapes. Ces points étapes permettent ensuite de naviguer dans les versions pour revenir à l'état du projet à un instant précis. Les points étapes sont appelés *commit*. 

#### Fonctionnement
Après une série de modifications (ajout, suppression ou modification de fichiers) dans un répertoire, il est nécessaire de les enregistrer dans l'index. Pour cela, il faut réaliser les étapes suivante : 

- Si ce n'est pas déjà fait, créer l'index de GIT pour le répertoire en question : `git init`
- Ajouter le ou les fichiers modifiés à l'index de GIT : `git add nom_du_fichier`
- Ajouter le commit en lui-même avec son commentaire : `git commit -m "mon commentaire"`

Lorsque tous les fichiers modifiés ont préalablement été ajoutés à l'index, il est possible de ne pas taper la commande `git add` mais directement la commande `git commit` en y ajoutant l'option `-a`. Par exemple :
	
	git commit -am "mon commentaire"
	
Le commentaire permettra aux autres contributeurs au projet ou à l'auteur plus tard de retrouver facilement certaines étapes du projet comme l'ajout d'une fonctionnalité. Il est donc important que le commentaire soit le plus précis possible. Il ne faut toutefois pas qu'il soit trop long au risque de perdre la personne faisant les recherches dans les descriptions.

### Consulter l'historique
Lorsque le projet progresse, les _commit_ s'accumulent. La consultation de l'historique des *commit* se fait avec la commande :

	git log

![Git Log](git_log.png)

La commande affiche la liste des *commit* de la branche sur laquelle nous sommmes (nous verrons les bracnches au chapitre suivant). Pour chaque *commit*, les informations suivantes s'affichent :

- le mot *commit* suivi d'un code complexe. Celui-ci est appelé le *SHA* et est un identifiant unique du *commit*.
- l'auteur du *commit* avec son nom suivi de de son adresse email.
- Le commentaire du *commit*.

Il est possible à tout moment de restaurer les fichiers telqu'ils étaient lors d'un *commit* en particulier. Pour cela, il faut utiliser la commande : 
	

### Les branches
