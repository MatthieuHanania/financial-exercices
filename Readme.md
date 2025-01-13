# Projets relatif au monde financier

Matthieu Hanania

## Description

Ce répertoire est constitué de 3 projets relatifs au monde financier.

### Riskfolio
> Riskfolio.ipynb

Ce projet consiste en une utilisation de la bibliothéque *risfolio* en python. Elle permet, pour des actions sur une période donnée, de calculer la stratégie optimale d'investissement en fonction du taux de risque choisi par l'utilisateur.

En entrée du projet, il est possible de fournir différentes actions d’entreprises. Le modèle va alors calculer le portefeuille optimal. 

Des actions qui fluctuent beaucoup ont un taux de risque plus élevé. Ainsi, en fonction des taux de risque, le portefeuille optimal va changer.

L’exemple utilisé dans le projet montre que, pour un investissement sans risque, il est conseillé d’investir beaucoup dans Orange, et pour un investissement plus risqué, il est conseillé d’investir dans Accor.


### Loi normale

> MonteCarlo\loi normale.ipynb  

 Ce projet est un exercice théorique.

Imaginons une action au prix actuel de 100 €, avec une volatilité annuelle de 20 %.   

On calcule sa volatilité journalière par 20% / sqrt(252) = 1.25%
252 étant le nombre de jours ouvrés

Prix du jour suivant = prix actuel × (1 + variation aléatoire)

Pour calculer la variation aléatoire, on suit une loi normale centrée en 0 et d’écart type 1,25 %.

À l’aide des simulations, on peut estimer le risque d’un portefeuille en calculant le nombre de simulations dont la valeur est en dessous d’un certain seuil.

En simulant 3 actions, aux valeurs initiales de 50, 100 et 150, on observe que dans 14 % des simulations, la valeur totale du portefeuille est inférieure à 270.

### MonteCarlo

> MonteCarlo\MonteCarlo.ipynb

Étude à nouveau du principe de Monte Carlo, cette fois en se basant sur un portefeuille composé d’actions réelles.
Cet exercice est basé sur la vidéo suivante https://www.youtube.com/watch?v=6-dhdMDiYWQ&list=PLqpCwow11-OqqfELduCMcRI6wcnoM3GAZ

Dans ce projet, l’évolution du portefeuille dépend de la moyenne des évolutions des actions au cours du temps, de leur covariance, et d’une variation aléatoire simulée chaque jour.
