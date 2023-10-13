# Création d'un dépôt GIT 
## Création d'un dépôt GIT en local
Dans la console, initialitialisation du dépôt:
```bash
git init
```
Cecicrée un dossier caché nommé ´.git´ qui contient tout l'histoire du projet. 
## Visualisation de l'état de GIT
```bash
git status
```
### Pour voir les fichiers et dossiers Unix

```bash
ls -a
```

## Pour ajouter un fichier à la future sauvegarde
Le -a permet d'affichier les dossier/fichiers cachés.
```bash
git add README.MD
```

## Pour effectuer la sauvegarde 
Les fichiers en attents de sauvegarde sont en vert.

Les fichiers en **staging** seront sauvés

```bash
git commit -m  "Message du commit" 
```
Un commit est une sauveguarde, on peut y accéder avec un 'git log' (affichage des identifiants des
sauvegardes et 'git show' (sans paramétre, affichage du dernier commit)

## Pour ajouter tous les fichiers en staging 

```bash
git add .
```
## Pour retirer un fichier du staging

```bash
git restore --staged README.md
```
Le fichier est sorti du `staging` et sera affiché en rouge avec `git status`

## Ajout d'un serveur distant

Nous allons utiliser un dépôt que l'on va créer sur github.com,
aprés connexion. Comme c'est un travail personnel, son URL sera de
ce type http://github.com/VOTRE_USERENAME/leNomDuProjet

Nous créons un new Repitory, puis nouscopions la clefs SSH : 
git@github.com:rammroumm2K/exe01html.git

Nous retournos dans notre git bash :
```bash
git remote add origin  git@github.com:rammroumm2K/exe01html.git
```
Pour voir si ça a fonctionné
```bash
git remote -v
```

##Envoi du projet 
```bash
git push origin main
```

## Récupération du projet

Si on souhaite récupérer toute la branche `main`

```bash
git pull origin main
```

Si on a effectué des modifations en local non voulues empéchant la récupération des fichiers(`merge error`).
On peut utiliser un `git stash` pour faire une pseudo sauvegarde et revenir au dernier commit
avant de réfaire un `git pull`

