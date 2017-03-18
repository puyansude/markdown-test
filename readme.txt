mkdir dossier
cd dossier
touch index.html
touch about.html

// Placer le dossier courant sous gestion de versions
git init
ls -la

// Ajouter un fichier à l agestion de versions
git add index.html

// Voir l'état des fichiers
git status

// Ajouter tous les fichiers du dossier courant 
git add .


git status

// Créer un point de restoration
git commit -m "révision 1"


git status

//Afficher les points de restoration
git log

// Modifier le contenu du fichier index.html

git status

// Note les changements ne sont pas mise en scène 'staged' pour un commit.  

// Il faudra faire un git add

// Ou bien, il est possible d'annuler les changements fait au fichier avec:

git checkout -- nomFichier

git add .

// Pour 'unstager' un fichier:

git reset HEAD nomFichier

// Pour "stager + commit" en une commande:
// Note: pas d'impact pour les nouveaux fichiers
git commit -a -m "révision 3"

 
// Suppression d'un fichier

1 - effacer le fichier
gat status

pour récupérer le fichier:

git checkout -- xyleFichierEffacerx


2 - git add leFichierEffacer
3 - git commit -m "J'ai effacé le fichier leFichierEffacer"






