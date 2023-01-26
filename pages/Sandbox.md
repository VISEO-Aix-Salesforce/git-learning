---
layout: default
---
[Menu](../index)

# Mise en place de la connexion à la sandbox

## Installer les extensions Salesforce pour VSCode

Ouvrez VSCode et accédez à l'onglet Extensions sur la gauche.

Tapez ensuite Salesforce Extension pack dans la barre de recherche, vous verrez une liste d'extensions cliquez sur *Salesforce Extension Pack*.

Après avoir cliqué sur *Salesforce Extension Pack*, vous verrez alors l'option d'installation de l'extension

## Installer l'interface de ligne de commande Salesforce

Vous pouvez télécharger la CLI Salesforce à partir d'ici https://developer.salesforce.com/tools/sfdxcli. La CLI Salesforce est également disponible pour MacOS, Windows et Linux.

Salesforce fournit également de la documentation avant d'installer la CLI Salesforce https://developer.salesforce.com/docs/atlas.en-us.sfdx_setup.meta/sfdx_setup/sfdx_setup_intro.htm.

## Assurez-vous que tout a été installé correctement

Ouvrons la palette de commandes pour nous assurer que les commandes SFDX s'affichent. Vous pouvez ouvrir la palette de commandes en appuyant sur *CTRL + SHIFT + P* sous Windows ou *CMD + SHIFT + P* sous MacOS.

Une autre option consiste à cliquer sur l'option *View* en haut, puis sur l'option *Command Pallette...*.

Accéder à la palette de commandes VSCode à l'aide de la vue
Dans la palette de commandes, tapez sfdx et vous devriez voir une liste d'options.

Options VSCode *sfdx* affichées après l'installation du pack d'extension Salesforce

## Autoriser une organisation

C'est ici que nous connectons VSCode à une organisation Salesforce, nous pouvons également avoir plusieurs connexions à différentes organisations.

Par exemple, vous pouvez connecter VScode à votre bac à sable de développement personnel et à vos organisations QA/UAT/Production.

Après avoir sélectionné *Authorize an Org*. Vous serez invité avec plus d'options en ce qui concerne le type de bac à sable auquel vous vous connectez.

VSCode Sélectionnez le type de bac à sable pour autoriser une commande d'organisation
Si vous autorisez votre organisation de production, sélectionnez *Production*, sinon sélectionnez l'option *Sandbox*.

> **Note**
>
> Si vous connectez du code Visual Studio à une organisation Trailhead, vous devez sélectionner *Production*.


L'étape suivante vous demandera d'entrer l'alias de cette connexion. Ceci est très utile lorsque vous avez plusieurs connexions à différentes configurations d'organisations.

Habituellement, j'essaie de donner un nom descriptif à l'Alias et d'appeler mes connexions selon les lignes de production/uat/dev afin que je sache à quelle organisation la connexion est destinée.

Cela aide lorsque je change de connexion car je peux voir le nom d'alias dans la barre bleue inférieure de VSCode qui m'indique l'organisation actuelle à laquelle je suis connecté.

Nom d'alias pour la connexion Salesforce dans vscode
Après avoir entré un nom d'alias, un onglet s'ouvrira dans votre navigateur par défaut où vous entrerez votre nom d'utilisateur et votre mot de passe.

Une fois connecté, un message vous demandera d'autoriser Salesforce CLI à accéder à votre organisation.

Cliquez sur *Allow*.

> **Astuce**
>
> Parfois, l'onglet peut mettre un certain temps à s'ouvrir. Vous devrez peut-être annuler l'autorisation et réessayer.


Autoriser l'accès VSCode à l'organisation Salesforce
Vous êtes maintenant connecté à votre organisation Salesforce, vous devriez voir le nom d'alias dans la barre bleue correspondre à celui que vous venez de créer.

[Menu](../index)
