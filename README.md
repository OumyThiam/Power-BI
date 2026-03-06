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
<img width="1875" height="1830" alt="image" src="https://github.com/user-attachments/assets/3de913fd-db3a-4d5b-9c5a-afc2e0972b06" />
Cette interface permet de piloter la performance commerciale globale en un coup d'œil. Elle centralise quatre indicateurs majeurs (CA, volume de commandes, quantités et panier moyen) complétés par une analyse temporelle et géographique. J'ai intégré une segmentation par catégorie de produit et un tableau de traçabilité détaillé pour assurer une lecture précise des données. L'interactivité est renforcée par des filtres dynamiques et des info-bulles personnalisées (tooltips) qui affichent des graphiques d'évolution au survol des régions, offrant ainsi un diagnostic rapide sans surcharger le visuel.

## Focus : Analyse des pertes (Commandes annulées)
<img width="1864" height="1790" alt="image" src="https://github.com/user-attachments/assets/78e1d21e-5732-40d5-8709-e630c123d410" />
Cette page a pour objectif d'identifier les zones de friction et de quantifier le manque à gagner. Trois indicateurs clés (KPI) permettent de mesurer immédiatement l'ampleur du phénomène : le nombre total d'annulations, leur montant financier et la part qu'elles représentent par rapport aux ventes globales. L'analyse est approfondie par un graphique en ruban qui suit l'évolution des annulations par produit au fil des trimestres, révélant ainsi les tendances saisonnières ou critiques. Une Treemap vient compléter cette vue pour isoler la part des pertes par catégorie de produit, tandis qu'un histogramme vertical compare le taux d'annulation entre les différentes régions. Cette interface permet de transformer des données de "pertes" en leviers d'action concrets pour améliorer le taux de transformation.

## Interactivité : Info-bulles contextuelles
<img width="1390" height="711" alt="image" src="https://github.com/user-attachments/assets/12218092-82df-4624-aaa0-529313a2e50f" />
Pour enrichir l’analyse sans complexifier l’interface, j’ai mis en place des pages d'info-bulles dynamiques qui s'activent au survol des données. Plutôt que de simples chiffres, l'utilisateur accède instantanément à une visualisation contextuelle, comme l'évolution temporelle précise du chiffre d'affaires pour une région donnée. Cette fonctionnalité permet un double niveau de lecture : une vue d'ensemble sur le graphique principal et un diagnostic détaillé via l'info-bulle, rendant l'exploration des données à la fois fluide et intuitive.






