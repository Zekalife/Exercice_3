#<p style="text-align:center;"> Présentation de GIT

## GIT 
GIT est un logiciel de gestion de version basé sur le modèle distribué. Développé par Linus Torvalds, l'auteur de Linux, il est l'un des plus utilisé actuellement et connais un succès grandissant. Le code peut être partagé directement entre deux développeur mais peut également être installé sur le site [GITHUB](http://github.com). Ce site héberge plusieurs millions de projet opensource pour la plupart. Il est toutefois possible d'ouvrir un compte payant pour y créer des dépôts (repository en anglais) privés.

Rentrons maintenant dans le fonctionnement de GIT

### Commit
Au fur et à mesure de la rédaction du code et la création des fichiers, il est nécessaire de créer des points étapes. Ces points étapes permettent ensuite de naviguer dans les versions pour revenir à l'état du projet à un instant précis. Les points étapes sont appelés *commit*. 

#### Fonctionnement
Après une série de modifications (ajout, suppression ou modification de fichiers) dans un répertoire, il est nécessaire de les enregistrer dans l'index. Pour cela, il faut réaliser les étapes suivante : 

- Si ce n'est pas déjà fait, créer l'index de GIT pour le répertoire en question : `git init`
- Ajouter le ou les fichiers modifiés à l'index de GIT : ``git add`` _nom du fichier_
- Ajouter le commit en lui-même avec son commentaire : `git commit -m "mon commentaire"`

Lorsque tous les fichiers modifiés ont préalablement été ajoutés à l'index, il est possible de ne pas taper la commande `git add` mais directement la commande `git commit` en y ajoutant l'option `-a`. Par exemple :
	
	git commit -am "mon commentaire"
	
Le commentaire permettra dans au autres contributeurs au projet ou à l'auteur plus tard de retrouver facilement certaines étapes du projet comme l'ajout d'une fonctionnalité. Il est donc important que le commentaire soit le plus précis possible. Il ne faut toutefois pas qu'il soit trop long au risque de perdre la personne faisant les recherches dans les descriptions.

### Consulter l'historique

### Les branches
