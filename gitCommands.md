# Les commandes principales de Git

Créer nouveau dépôt dans le dossier actuel
    git init 

Cloner un dépôt

    git clone /path/
    git clone username@host:/path/

Ajouter des fichiers au prochain commit
    git add *
    git add .
    git add nomfichier.html

Créer un "commit"(snapshot) des fichiers ajoutés précédemment
    git commit -m "votre message"

Envoyer votre commit sur le dépôt distant
    git push origin NomDeBranche
    git push origin Master

Ajouter le point d'origine(en ligne) de votre branche
    git remote add origin <server>

Créer nouvelle branche
    git checkout -b NomDeBranche

Changer de branche
    git checkout NomDeBranche
    git checkout Master

Supprimer une branche (qui a été fusionnée)
    git branch -d NomDeBranche

Supprimer la branche du dépôt en ligne
    git push origin --delete NomDeBranche

Lister les branches disponible en local (et les origines en ligne)
    git branch -a

Récupérer les informations(en-têtes) des branches/dépôts en ligne
    git fetch --all

Propager les informations que l'on possède (/!\ Dangereux)
    git fetch -all -prune

Supprimer les modifications d'un fichier en local 
    git checkout -- nomfichier

