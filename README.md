# Prédiction du churn bancaire

Projet personnel de classification supervisée : prédire si un client va quitter une banque (churn) à partir de ses caractéristiques.

## Données
Jeu de données public de 10 000 clients d'une banque (CreditScore, âge, pays, solde, nombre de produits, ancienneté, etc.), avec une variable cible "Exited" (1 = le client a quitté la banque, 0 = il est resté).

## Démarche
- Nettoyage des données (suppression des identifiants non pertinents)
- Encodage des variables catégorielles (pays, genre)
- Séparation entraînement / test (80 % / 20 %)
- Standardisation des variables pour les modèles sensibles à l'échelle

## Modèles comparés
| Modèle | Précision (accuracy) |
|---|---|
| Régression logistique | 0.808 |
| Arbre de décision | 0.861 |
| SVM (noyau RBF) | 0.861 |

L'arbre de décision et le SVM obtiennent les meilleures performances, avec une nette amélioration par rapport à la régression logistique.

## Outils
Python — pandas, scikit-learn, matplotlib, seaborn

## Notebook
Voir `churn_bancaire.ipynb` pour le code complet (chargement des données, préparation, entraînement des modèles, matrice de confusion et comparaison graphique).
