# Création d'un dépôt GIT 
## Créatio d'un dépôt GIT en local
Dans la console, initialitialisation du dépôt:
```bash
git init
```
## Visualisation de l'état de GIT
```bash
git status
```
### Pour voir les fichiers et dossiers Unix

```bash
ls -a
```

## Pour ajouter un fichier à la future sauvegarde

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

´´´bash
git add .
´´´

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
