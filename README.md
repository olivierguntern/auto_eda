# Comprehensive EDA Processor

![EDA Processor Banner](banner.png) <!-- Optionnel : Ajouter une image de bannière -->

## Table des Matières
- [Aperçu](#aperçu)
- [Fonctionnalités](#fonctionnalités)
- [Installation](#installation)
- [Configuration](#configuration)
- [Utilisation](#utilisation)
- [Résultats](#résultats)
- [Résumé Global](#résumé-global)
- [Dépannage](#dépannage)
- [Contribution](#contribution)
- [Licence](#licence)
- [Remerciements](#remerciements)

## Aperçu

Le **Comprehensive EDA Processor** est un script Python robuste et flexible conçu pour effectuer une Analyse Exploratoire des Données (EDA) approfondie sur divers ensembles de données. Optimisé pour des environnements comme Kaggle, il supporte plusieurs formats de données, automatise le nettoyage des données, génère des visualisations informatives et produit des rapports détaillés aux formats JSON et Markdown. De plus, un résumé global concis est généré pour faciliter la compréhension rapide des caractéristiques de chaque DataFrame analysé.

## Fonctionnalités

- **Support Multi-Format :** Gère les fichiers CSV, JSON, Excel (`.xlsx`) et Parquet (`.parquet`).
- **Optimisation des Performances :** Utilise le traitement parallèle avec `ThreadPoolExecutor` pour un chargement plus rapide des données.
- **Nettoyage de Données Avancé :**
  - Détection et suppression des enregistrements dupliqués.
  - Gestion des valeurs manquantes avec imputation automatique.
  - Encodage des variables catégorielles avec `LabelEncoder`.
  - Normalisation des caractéristiques numériques avec `StandardScaler` ou `MinMaxScaler`.
- **Détection des Outliers :** Identifie et visualise les outliers dans les colonnes numériques.
- **Visualisations Complètes :**
  - Histogrammes interactifs, boxplots et matrices de corrélation avec Plotly.
  - Pairplots avec Seaborn pour explorer les relations entre variables.
  - Analyse des séries temporelles pour les ensembles de données contenant des colonnes de date.
- **Rapports Automatisés :**
  - Génère des rapports détaillés en formats JSON et Markdown.
  - Inclut les types de données, les valeurs manquantes, les statistiques descriptives, les comptes d'outliers, etc.
- **Résumé Global :** Compile un résumé concis de tous les DataFrames analysés, facilitant la compréhension rapide de leurs caractéristiques.
- **Journalisation :** Journalisation détaillée du processus EDA pour un débogage et un suivi faciles.
- **Fichier de Configuration :** Paramètres personnalisables via `config.yaml` sans modifier le code principal.
- **Exportation des Données Nettoyées :** Sauvegarde les ensembles de données nettoyés au format CSV pour une utilisation ultérieure.

## Installation

### Prérequis

- Python 3.6 ou supérieur
- Gestionnaire de paquets `pip`

### Guide Étape par Étape

1. **Cloner le Répertoire :**

   ```bash
   git clone https://github.com/votreutilisateur/eda-processor.git
   cd eda-processor
