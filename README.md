# Résumé Automatique de Texte avec Encoder-Decoder

Ce projet met en œuvre un modèle de résumé automatique de texte utilisant une architecture encoder-decoder et des techniques d'extraction de phrases clés.

## Installation

1. Assurez-vous d'avoir Python 3.7 ou une version ultérieure installée.
2. Installez les bibliothèques nécessaires :

## Utilisation

1. **Préparer les données:**
    - Téléchargez le jeu de données CNN/Daily Mail à partir de Hugging Face Datasets : `datasets load abisee/cnn_dailymail`
    - Exécutez le code dans la section "Téléchargez et préparez un jeu de données" pour nettoyer, lemmatiser et diviser les données en ensembles d'entraînement, de validation et de test.
2. **Entraîner le modèle:**
    - Exécutez le code dans la section "Construction du modèle Encoder-Decoder" pour entraîner le modèle BART. 
    - Ajustez les paramètres d'entraînement tels que le nombre d'epochs et le taux d'apprentissage si nécessaire.
3. **Générer des résumés:**
    - Exécutez le code dans la section "Génération de résumés" pour générer des résumés abstraits à partir du jeu de test.
    - Utilisez la fonction `generate_summary_abstractive` pour générer un résumé pour un nouvel article.
4. **Évaluer les performances:**
    - Exécutez le code dans la section "Évaluation des performances" pour calculer les scores ROUGE et BLEU des résumés générés par rapport aux résumés de référence.

## Extraction de phrases clés (Modèle extractif)

- Le code dans la section "Modèle de résumé extractif" utilise BERT pour extraire les phrases clés d'un texte.
- La fonction `extract_key_phrases` peut être utilisée pour extraire les phrases clés d'un nouveau texte.

## Remarques

- Le code est optimisé pour s'exécuter sur un GPU si disponible.
- Les chemins d'accès aux fichiers et les noms de variables peuvent nécessiter des ajustements en fonction de votre environnement.


## Auteurs

Sogo Armel Emmanuel, Ouedraogo Relwindé Guillaume Victorien


## Licence

[MIT License or other license]

