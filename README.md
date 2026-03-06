Analyse de Performance Commerciale et Litiges : Dashboard Power BI
À propos du projet

Ce projet est né de la volonté de transformer des données de ventes brutes, souvent difficiles à exploiter, en un outil de pilotage stratégique fluide et visuel. L'enjeu était de taille : passer d'un fichier CSV plat à un modèle de données relationnel capable de répondre à des questions métier précises, tout en offrant une expérience utilisateur moderne.

L'objectif principal est double : monitorer la croissance du chiffre d'affaires et disséquer les points de friction via l'analyse approfondie des commandes annulées.
Ce que j'ai réalisé
1. La fondation : Nettoyage et Structuration (Power Query)

Avant de créer des graphiques, j'ai passé du temps "sous le capot" pour m'assurer de la fiabilité des chiffres :

    Audit de données : Analyse de la qualité et de la distribution pour éliminer toute anomalie.

    Normalisation : J'ai déconstruit la table unique pour créer un schéma en étoile avec des tables de référence pour les Clients, les Produits et les Régions.

    Professionnalisation : Renommage complet des colonnes pour utiliser un vocabulaire métier clair et accessible.

2. L'intelligence : Mesures DAX et Modélisation

J'ai conçu une couche de calculs personnalisés pour donner du sens aux données :

    Pilotage standard : Création de mesures pour le CA total, le volume de commandes et le panier moyen.

    Analyse avancée des annulations : Utilisation de fonctions calculées pour isoler précisément l'impact financier des commandes au statut "Cancelled".

3. L'expérience : Design et Navigation

L'esthétique sert ici la compréhension. J'ai choisi un thème sombre ("Loomy Lime") pour faire ressortir les indicateurs clés:

    Navigation intuitive : Un menu latéral permet de naviguer entre la vue "Ventes" et la vue "Annulations".

    Détails au survol : Mise en place d'info-bulles (tooltips) qui affichent l'historique de vente d'une région ou d'un produit sans quitter la page principale.

Aperçu visuel
Vue d'ensemble : Pilotage des ventes

Cette page permet de comprendre en un coup d'œil d'où vient le chiffre d'affaires. Le tableau détaillé en bas de page assure la traçabilité de chaque transaction.
Focus : Analyse des pertes (Commandes annulées)

Ici, on cherche à comprendre le "pourquoi". Le graphique en ruban montre l'évolution des annulations par produit sur l'année, permettant d'identifier des tendances saisonnières ou des problèmes récurrents.
Interactivité : Info-bulles contextuelles

Pour éviter de multiplier les graphiques, j'ai intégré des graphiques secondaires qui n'apparaissent que lorsqu'on survole une donnée précise.
Fonctionnalités "Expert" intégrées

    Sécurité des données (RLS) : Configuration de rôles pour que chaque responsable de région ne voie que ses propres chiffres.

    Accessibilité mobile : Création d'une mise en page spécifique pour consulter les KPI depuis un smartphone.

    Filtres dynamiques : Utilisation de signets (bookmarks) pour segmenter instantanément le parc produit (Mobiles vs Bureautique).