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

// Note les changements ne sont mise en scène 'staged' pour un commit.  

// Il faudra faire un git add

// Ou bien, il est possible d'annuler les changements fait au fichier avec:

git checkout -- nomFichier

git add .

// Pour 'unstager' un fichier:

git reset HEAD nomFichier

// Pour "stager + commit" en une commande:
git commit -a -m "révision 3"
 

// Déplacer la tête 'HEAD' à un autre point dans le temps:
git reset --hard 9880b6624ec75f026ed9f62ffba93d8b93f69d51

// Lister les fichiers d'un dépot:
git ls-tree HEAD
git ls-tree master

// Lister les fichiers de master - 3 commits
git ls-tree master~3 

// Exemples de logs
git log --oneline

////
// Afficher les modifications d'un commit:
git show cfd3397e

commit cfd3397e930b8484fc02ed93a7127393550008c8
Author: Alain <alain@MacBook-Pro.local>
Date:   Sun Mar 19 20:46:54 2017 -0400

    Mise à jour du fichier readme

diff --git a/readme.txt b/readme.txt
index 2a86175..a492a04 100644
--- a/readme.txt
+++ b/readme.txt
@@ -50,7 +50,8 @@ git reset HEAD nomFichier
 git commit -a -m "révision 3"
  
 
-
+// Déplacer la tête 'HEAD' à un autre point dans le temps:
+git reset --hard 9880b6624ec75f026ed9f62ffba93d8b93f69d51

///--------------------------

// Créer une branche et rester sur la branche courant
git branch nom_branche

// Créer une branche et se déplacer sur la nouvelle branche
git branch -b nom_branche


// Déplacer HEAD vers une branche
git checkout nom_branche

// Renommer une branche (--move)
git branch -m nom_courant nouveau_nom


// Effacer une branche (--delete, se placer sur la branche 'master' avant d'effacer)
git branch -d nom_branche_a_effacer

// Afficher les différences entre 2 branches:
git diff master...ajout_fn1

// Ajout du nom de la branche dans l'invite (prompt) du système



////======================
// github
// https://stackedit.io/editor


