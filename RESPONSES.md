Question 1 (compte-rendu) : Que contient le répertoire .git/ ? À quoi sert-il ?

Le répertoire .git/ contient notre repo local qui permet de faire de la gestion de version avec GIT


Question 2 (compte-rendu) : Quelle est la différence entre un fichier untracked, staged et
committed ?

Le fichier untracked est juste dans le dossier de travail.
Le fichier staged est indexé pour être ajouté au prochain commit.
Et le fichier committed est un fichier qui a été envoyé au repo local


Question 3 (compte-rendu) : Quelle est la différence entre git diff et git diff --staged ? À
quel moment utiliseriez vous chacune ?

git diff compare mon dossier de travail avec la staging area > Pour vérifier ce que j'ai modifié avant de faire un git add
git diff --stage compare la staging area avec le dernier commit > Pour vérifier ce qu'on s'apprête à commit


Question 4 (compte-rendu) : Quelle est la différence entre git revert et git reset ? Dans
quel cas utiliser l'un ou l'autre ?

Le revert permet de revenir à un commit précédent alors que le reset permet de retourner à un staged précédent


Question 5 (compte-rendu) : Qu'est-ce qu'un fast-forward merge ? Dans quel cas Git
effectue-t-il un fast-forward plutôt qu'un merge commit ?

Un fast-forwar merge est une fusion rapide de 2 branches.
Git utilise un merge commit s'il y a eu des modifications/commit sur la main avant la fusion


Question 6 (compte-rendu) : Pourquoi est-il recommandé de supprimer les branches une fois
fusionnées ? Quelle différence entre -d et -D ?

Il est recommandé de supprimer les branches pour garder un historique/répertoire propre et donc plus lisible
Le -d va s'arrêter s'il rencontre un soucis (merge pas finis) alors que le -D va forcer la suppression


Question 7 (compte-rendu) : Décrivez en vos propres mots ce qu'est un conflit Git, pourquoi il
survient, et quelles sont les étapes pour le résoudre.

Un conflit Git c'est un conflit lors d'un merge. Cela ce produit qu'il y a 2 versions différentes d'un même fichier sur des branches différentes.
Pour résoudre le conflit, il faut utiliser un outils pour comparer les différences entre les 2 fichiers, choisir les bouts de codes ou les fichiers qui vont être garder puis relancer une merge
