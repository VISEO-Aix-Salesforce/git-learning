---
layout: default
---

# Branching Strategy
 
 ![Octocat](https://github.com/VISEO-Aix-Salesforce/git-learning/blob/main/assets/images/branchingStrategy.png)

Au lieu d'une seule branche principale, ce workflow utilise deux branches pour enregistrer l'historique du projet. 
La branche principale stocke l'historique officiel des versions et la branche develop sert de branche d'intégration pour les fonctionnalités. 
Il est également pratique de baliser tous les commits de la branche principale avec un numéro de version.


La première étape consiste à compléter la main par défaut avec une branche develop. 
Pour ce faire, un moyen simple consiste pour un développeur à créer localement une branche de développement vide et à la pousser vers le serveur.

Cette branche contiendra l'historique complet du projet, alors que main contiendra une version abrégée. 
Les autres développeurs doivent maintenant cloner le référentiel central et créer une branche de suivi pour develop.

Chaque nouvelle fonctionnalité doit résider dans sa propre branche, qui peut être poussée vers le référentiel central pour la sauvegarde/collaboration. 
Mais, au lieu de bifurquer de main, les branches de fonctionnalités utilisent develop comme branche parent. 
Lorsqu'une fonctionnalité est terminée, elle est fusionnée dans develop. 
Les fonctionnalités ne doivent jamais interagir directement avec main.
