Analyse de Performance Commerciale : Dashboard Power BI

Ce projet est né de la volonté de transformer des données de ventes brutes, souvent difficiles à exploiter, en un outil de pilotage stratégique fluide et visuel. L'enjeu était de passer d'un fichier CSV plat à un modèle de données relationnel capable de répondre à des questions métier précises, tout en offrant une expérience utilisateur moderne.

L'objectif principal est double : monitorer la croissance du chiffre d'affaires et disséquer les points de friction via l'analyse approfondie des commandes annulées.
# Analyse de Performance Commerciale : Dashboard Power BI

[![Dataset](https://img.shields.io/badge/dataset-sales_2.csv-blue)](./sales_2.csv) [![Power BI](https://img.shields.io/badge/Power--BI-ready-4c1)](https://powerbi.microsoft.com/) [![Licence](https://img.shields.io/badge/license-MIT-lightgrey)](./LICENSE)


## Ce que j'ai réalisé

1. Nettoyage et Structuration (Power Query)

- Audit de données : vérification de la qualité et traitement des anomalies.
- Normalisation : création d'un schéma en étoile (dimensions Clients, Produits, Régions).
- Renommage des colonnes pour un vocabulaire métier clair.

2. Mesures DAX et Modélisation

- Mesures classiques : CA total, nombre de commandes distinctes, panier moyen.
- Analyses des annulations : mesures filtrées sur `OrderStatus = "Cancelled"` pour estimer l'impact financier.

3. Design et Navigation

- Thème visuel adapté pour faire ressortir les KPI.
- Navigation et info-bulles pour gagner en ergonomie et ne pas surcharger les pages.

## Aperçu visuel

## Vue d'ensemble : Pilotage des ventes
![alt text](image.png)
Cette page permet de comprendre en un coup d'œil d'où vient le chiffre d'affaires. Le tableau détaillé en bas de page assure la traçabilité de chaque transaction.

## Focus : Analyse des pertes (Commandes annulées)
![alt text](image-1.png)
Ici, on cherche à comprendre le "pourquoi". Le graphique en ruban montre l'évolution des annulations par produit sur l'année, permettant d'identifier des tendances saisonnières ou des problèmes récurrents.
## Interactivité : Info-bulles contextuelles
![alt text](image-2.png)
Pour éviter de multiplier les graphiques, j'ai intégré des graphiques secondaires qui n'apparaissent que lorsqu'on survole une donnée précise.





