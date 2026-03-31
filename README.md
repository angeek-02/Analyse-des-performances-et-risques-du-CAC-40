(Projet en cours)
Le travail a été réalisé sur l'environnement Google Colab.

Phase 1: Recherche & collecte de données
- Récupération des noms et indices des entreprises constituant le CAC 40
- "Camouflage" web pour avoir accès aux données de Wikipédia pour l'extraction
- Récupération des données et gestion des erreurs

Phase 2: Nettoyage des données
- Transformation des données récupérées en tableau structuré (sous forme de liste dataframe)
- Ajout de l'indice du CAC 40 (^FCHI) à la colonne 'Ticker' pour le benchmark

Phase 3: Exportation vers SQL
- Création d'une table "Prices" pour l'intégrer dans la base de sonnées SQL de l'entreprise
- Automatisation de la date (On compte 10 ans à partir du jour présent)
  Ces étapes sont importantes pour cadrer l'extraction des prix sur Yahoo Finance.

Phase 4: Extraction des données sur yfinance
- Gestion des erreurs
- Sélection des informations pertinentes pour notre analyse
- Formatage des données pour une exploitation plus facile.

Phase 5: Exploitation des données
- Extraction de données via la fonction sql_query
- Calcul des rentabilités journalières
- Calcul du bêta de chaque entreprise
- Calcul du Ke selon le modèle du MEDAF

Phase 6: Visualisation des données (en cours)
- Utilisation de Power BI pour la visualisation des entreprises du CAC qui ont réalisés les meilleurs performances, mais aussi celles qui sont les plus risqués (grande sensibilité au marché)
- Analyse des données
