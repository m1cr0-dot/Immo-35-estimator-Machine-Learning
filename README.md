# 🏡 Estimateur Immobilier Ille-et-Vilaine (35)

Une application de Data Science interactive permettant d'estimer le prix de vente de maisons et d'appartements en Ille-et-Vilaine grâce au Machine Learning.

🔗 **[Accéder à l'application en ligne](https://immo-35-estimator-ml.streamlit.app/)**

## 📋 Description du Projet

Ce projet a pour but de prédire la valeur vénale d'un bien immobilier en se basant sur ses caractéristiques intrinsèques (surface, pièces, terrain) et sa localisation géographique.

Le modèle a été entraîné sur des données réelles de transactions immobilières dans le département 35. Il intègre un feature engineering spatial calculant notamment la distance aux pôles économiques majeurs (Rennes et Saint-Malo).
Lien dataset (kaggle): https://www.kaggle.com/datasets/cheneblanc/housing-prices-35-fr

## 🧠 Performance du Modèle

Le moteur de prédiction repose sur un algorithme de **Random Forest Regressor** optimisé.

* **Score R² :** ~0.75 (Le modèle explique 75% de la variance des prix)
* **Précision Moyenne (MAPE) :** ~26% (sur l'ensemble des biens, ruraux inclus)
* **Erreur Absolue Moyenne (MAE) :** ~36 000 €

## 🛠️ Stack Technique

* **Langage :** Python
* **Machine Learning :** Scikit-Learn (Random Forest, Pipeline, RandomizedSearchCV)
* **Data Processing :** Pandas, NumPy
* **Interface Web :** Streamlit
* **Déploiement :** Streamlit Community Cloud

## 🚀 Installation locale

Si vous souhaitez faire tourner le projet sur votre propre machine :

1.  **Cloner le dépôt :**
    ```bash
    git clone [https://github.com/m1cr0-dot/Immo-35-estimator-Machine-Learning.git](https://github.com/m1cr0-dot/Immo-35-estimator-Machine-Learning.git)
    cd immo-bretagne-estimator
    ```

2.  **Installer les dépendances :**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Lancer l'application :**
    ```bash
    streamlit run app.py
    ```

Une page web s'ouvrira automatiquement dans votre navigateur à l'adresse `http://localhost:8501`.

## 👤 Auteur

Projet réalisé par **[Ton Prénom Nom]** dans le cadre d'un projet personnel de Data Science (Niveau M1).
