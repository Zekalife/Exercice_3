#<p style="text-align:center;"> Présentation de GIT

## Concept
<div style="text-align:justify;">
GIT est un gestionnaire de version de fichier. Principalement utilisé par les équipes de développement de logiciels, les gestionnaires de versions de fichiers permettent de garder une trace des modifications effectuées sur les différents fichiers d'un projet. Cela est très utile lorsque de nombreuses personnes travaillent ensemble sur un projet important.
Les principales fonctionnalités de ce type de gestionnaires sont :

* Enregistrement des différentes version de chaque fichier.
* Affichage des modifications effectuées entre deux version d'un fichier.
* Enregistrement des noms des personnes faisant les modifications.
* Création de branches de développement pour mettre au point une nouvelle fonctionnalité par exemple et ne l'intégrer dans la branche principale que lorsque a nouvelle fonctionnalité est entièrement finalisée et testée.

ce type de logiciel permettent également de suivre les évolutions de tout type de document autre que ceux directement liés au développement. Ils peuvent être utile par exemple, au rédacteur d'un ouvrage de revenir à l'état initial d'un chapitre s'il n'est pas satisfait des modifications.

Il existe deux principaux types de logiciel de gestion de version :

* Le modèle centralisé : les fichiers sont hébergés sur un serveur central. Chaque client accéde au serveur pour obtenir les fichiers et les informations sur les versions. A chaque modification, celle-ci doit être renvoyé vers le serveur pour être redistribuée vers les autres clients. 
* Le modèle distribué : chaque client possède l'intégralité des ficheirs sur son disque dur et la gestion des version est effectué localement. Elles sont partagées entre les clients lors d'opération de synchronisation.



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
