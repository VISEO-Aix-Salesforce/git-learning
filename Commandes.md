---
layout: default
---

# Commandes GIT
        
## Cloner un projet à pratir d'un repository

la Commande **Git Clone** permet de copier le repository d'un projet en local lors du demarrage d'un projet.

```js
Git clone https://github.com/<repository>/<Projet.git>
```

## Gestion des Branches 

La commande **Git Branch** permet de Créer, Lister ou supprimer des branches dans le projet 

```js
//Pour afficher la liste des branches du projet, la branche active est en général affichée en vert avec un asterix
Git Branch
```

```js
//Pour créer une branche sans faire de Checkout
Git Branch <newBranchName>
```

```js
//Pour supprimer une branche
Git Branch –d <branchname>
```

## Checkout 

La commande **Git Checkout** permet de changer la branche sur laquelle on travaille

```js
//Pour basculer de la branche courante sur la branche branchname
Git Checkout <branchname>
```

> _Astuce: Avec l'option -b vous pouvez créer a la volée une nouvelle branche et la passer en Branche courante_
> ```js
> Git Checkout –b <branchname>
> ```

## Status 

La commande **Git Status** permet d'afficher les différences entre la branche courante et les fichiers commités dans le dépôt (Repository).

```js
Git Status  
```

## Add 

La commande **Git Add** permet de faire entrer de nouveaux fichiers dans le flux d'indexation de git (Staging). Les fichiers ajoutés a l'aide de cette commande seront pris compte dans le prochain commit. Lorsqu'un fichier est modifié suite a son indexation, il faut refaire un Add pour prendre en compte la dernière version lors du prochain Commit.

```js
//Pour ajouter le fichier filename dans l'index Git
Git add <fileName> 
```

> _Astuce: Vous pouvez utiliser les wildcards (*) pour ajouter plusieurs fichiers à la fois_
> ```js
> //Pour ajouter tous les fichiers ajoutés ou modifiés dans l'indexation
> Git add . 
> ```

## Commit 

La commande **Git Commit** permet d'enregistrer les fichiers indexés dans le dépôt. Il doit s'accompgner d'un message decrivant les modifications apportées.
Le nouveau commit se place en haut de la branche courante (HEAD).

```js
//Pour faire un commit avec un message
Git Commit -m "JIRA50126 - J'ai fait ces trucs" 
```

## Merge

La commande **Git Merge** permet de fusionner deux branches de developpement distinctes. Les commits effectués sur la branche indiquée viendrons se rajouter en un commit en haut de la branche courante.

```js
Git Merge <branchetomerge>
```

> _Astuce: Pour ajouter un message de commit lors d'un merge utiliser l'option -m_
> ```js
> Git Merge <branchtomerge> -m "Message de Merge"
> ```

## Pull

La commande **Git Pull** permet d'intégrer les modification d'une branche distante dans la branche locale courante.

```js
//Pour faire un merge de la branche distante dans la branche locale
Git Pull
```


## Push

La commande **Git Push** permet de mettre à jour les branches distantes avec les modifications effectuées en local.
Pour eviter les pertes, il est conseillé de toujours faire un Pull et de resoudre les conflits avent de faire un Push.

```js
Git Push
```

## Fetch

La commande **Git Fetch** permet de recuppérer les modification d'une branche distante en local mais contrairement à un Pull ne va pas effectuer de merge.
Cette commande est utile lorsqu'il y a beaucoup de modifications et qu'un merge global pourrait entrainer la gestion de beaucoup de conflits en même temps.

```js
Git Fetch
```

# Références externes

Pour aller plus loin avec une liste plus détaillée des commandes Git
[Référence Git](https://git-scm.com/docs)
