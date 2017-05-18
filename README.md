# poc-gitflow
# initialisation
git flow init
git branch
git flow feature start homepage
git branch

# création de d'une feature
vim index.html
git add index.html
git commit "add html file"
git commit -m "add html file"
git flow feature publish homepage
git flow feature finish homepage
git branch

# création d'une release
git flow release start 1.1.0
git flow release finish 1.1.0
git push --tags
git push origin master
git push origin develop

# création d'un hotfix
git flow hotfix start title
vim index.html
git add .
git commit -m "changement du titre"
git flow hotfix finish
git push --tags
git push origin master
git push origin develop

# log
git log --graph --oneline --first-parent develop
