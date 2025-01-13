# Projets relatif au monde financier

Matthieu Hanania

## Description

Ce repertoire est constitué de 3 projets relatifs au monde financiers

### Riskfolio
> Riskfolio.ipynb

Ce projet consiste en une utilisation de la bibliothéque *risfolio* en python. Elle permet, pour des actions sur une période données, de calculer la stratégie optimale d'investissement en fonction du taux de risque choisi par l'utilisateur. 

En entrée du projet, il est possible de fournir différentes actions d'entreprises. 
Le modèle va alors calculer le portefeuil optimal. 

Des actions qui fluctuent beaucoup, ont un taux de risque plus élevés. Ainsi, en fonction des taux de risques, le portefeuil optimal va changé.

L'exemple utilisé dans le projet montre que pour un investissement sans risque, il est conseillé d'investir beaucoup dans Orange, et pour un investissement plus risqué, il est conseillé d'investir dans Accor


### Loi normale

> MonteCarlo\loi normale.ipynb  

Ce projet est un exercice théorique, 

Imaginons une action au prix actule de 100€, une volatilité annuelle de 20%.     

On calcul sa volatilité annuelle par 20% / sqrt(252) = 1.25%
252 étant le nombre de jours ouvrés

Prix du jour suivant = prix actuel * (1+variation aléatoire)

Pour calculer la variation aléatoire on suit une loi normale centrée en 0 d'écart type 1.25%

A l'aide des simulations, on peut estimer le risque d'un portefeuille en calculant le nombre de simulations dont la valeurs est en dessous d'un certain seuil. 

En simulant 3 actions, aux valeurs initiales de 50, 100 et 150, dans 14% des simulations, la valeur totale du portefeuille est inférieure à 270

### MonteCarlo

> MonteCarlo\MonteCarlo.ipynb

Etude à nouveau du principe de Monte Carlo, cette fois en se basant sur un portefeuille composé d'action réelles. 
Cet exercice est basé sur la vidéo https://github.com/MatthieuHanania/financial-exercices/tree/main

Dans ce projet, l'évolution du portefeuille dépend de la moyenne d'évolutions des actions au cours du temps, de leurs covariance, et d'une variation aléatoire simulé chaque jour