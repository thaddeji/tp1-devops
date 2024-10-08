# tp1-devops

Comment vérifier la configuration actuelle de Git sur votre machine, notamment le nom
d’utilisateur et l’adresse e-mail ?
git config --global user.name
git config --global user.email
Comment modifier votre adresse e-mail si vous l'avez mal configurée lors de l'installation
de Git ?
git config --global user.email "nouvelle.adresse@email.com"
Si vous avez oublié de créer un fichier README.md lors de l'initialisation du projet,
comment pouvez-vous l'ajouter après coup et commiter les changements ?
touch README.md
Comment définir un dépôt distant si vous n'en avez pas configuré un lors de la création
du projet ?
 Créer le dépôt distant sur GitHub, GitLab, ou une autre plateforme
 SSH : git@github.com:votre-nom-utilisateur/mon-projet.git
 Ajouter le dépôt distant à votre projet local
git remote add origin git@github.com:talelhaddeji/mon-projet.git
Vérifier que le dépôt distant a été ajouté correctement
git remote -v
Pousser les changements vers le dépôt distant
git push -u origin main
Comment annuler les modifications locales d'un fichier avant de les ajouter à l'index ?
git checkout -- monfichier.txt
Comment visualiser les fichiers qui sont prêts à être commités dans Git (staging) ?
git status
Comment suivre (track) un dépôt distant et récupérer toutes les branches de ce dépôt ?
Ajouter le dépôt distant
git remote add origin <URL-du-dépôt-distant>
 Récupérer toutes les branches
 git fetch origin
Vérifier les branches récupérées
git branch -a
 Créer des branches locales à partir des branches distantes
 git checkout -b branch1 origin/branch1
Mettre à jour les branches locales
git puComment supprimer une branche locale après l'avoir fusionnée dans main?
git branch -d feature-branch
Comment interrompre un rebase en cours si vous avez commis une erreur ?
git rebase --abort
Comment lister les commits qui vont être rebasés avant de lancer un rebase ?
git log --oneline main..feature-branch
Comment afficher la liste des branches actives et en cours de développement dans 
Gitflow ?
git branch -a
