# 🏡 Estimateur Immobilier Ille-et-Vilaine (35)

Une application de Data Science interactive permettant d'estimer le prix de vente de maisons et d'appartements en Ille-et-Vilaine grâce au Machine Learning.

🔗 **[![Streamlit App](https://immo-35-estimator-ml.streamlit.app/)]**

<p align="left"> 
    •<a href="#français">🇫🇷 Lire en Français</a> <br>•
    <a href="#english">🇬🇧 Read in English</a>
</p>

<a id="français"></a>
## 📋 Description du Projet

Ce projet a pour but de prédire la valeur vénale d'un bien immobilier en se basant sur ses caractéristiques intrinsèques (surface, pièces, terrain) et sa localisation géographique.

Le modèle a été entraîné sur des données réelles de transactions immobilières dans le département 35. Il intègre un feature engineering spatial calculant notamment la distance aux pôles économiques majeurs (Rennes et Saint-Malo).
Lien dataset (kaggle): https://www.kaggle.com/datasets/cheneblanc/housing-prices-35-fr

> **Pourquoi ce département ?**
>  Ce projet privilégie l'utilisation de données réelles plutôt que synthétiques. Bien que j'aie initialement envisagé d'analyser Paris ou Bordeaux, les datasets disponibles (sur Kaggle) étaient majoritairement générés par IA. J'ai donc sélectionné ce département car il offrait un jeu de données authentique et exploitable.

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
    git clone "https://github.com/m1cr0-dot/Immo-35-estimator-Machine-Learning.git"
    cd Immo-35-estimator-Machine-Learning
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

Projet réalisé par **Matteo CUNHA** dans le cadre d'un projet personnel de Data Science.


---

<a id="english"></a>
## 🇬🇧 Project Description

An interactive Data Science application designed to estimate the selling price of houses and apartments in Ille-et-Vilaine (France) using Machine Learning.

🔗 **[![Streamlit App](https://immo-35-estimator-ml.streamlit.app/)]**

### 📋 Context & Objectives
The goal of this project is to predict the **Market Value** of a property based on its intrinsic features (living area, number of rooms, land size) and its geographical location.

The model was trained on real estate transaction data from the department 35. It includes spatial feature engineering, specifically calculating distances to major economic hubs (Rennes and Saint-Malo).
* **Dataset Source (Kaggle):** [Housing Prices 35 FR](https://www.kaggle.com/datasets/cheneblanc/housing-prices-35-fr)

> **Why this specific region ?**
>  This project prioritizes **real-world data** over synthetic datasets. While I initially considered analyzing Paris or Bordeaux, the available datasets were mostly AI-generated. I selected this department because it provided an authentic dataset, allowing for genuine exploratory data analysis (EDA).

### 🧠 Model Performance
The prediction engine is built on an optimized **Random Forest Regressor**.

* **R² Score:** ~ 0.75 (The model explains 75% of the price variance)
* **Mean Absolute Percentage Error (MAPE):** ~ 26% (across all properties, including rural areas)
* **Mean Absolute Error (MAE):** ~ 36,000 €

### 🛠️ Technical Stack
* **Language:** Python
* **Machine Learning:** Scikit-Learn (Random Forest, Pipeline, RandomizedSearchCV)
* **Data Processing:** Pandas, NumPy
* **Web Interface:** Streamlit
* **Deployment:** Streamlit Community Cloud

### 🚀 Local Installation
To run the project on your local machine:

1. **Clone the repository:**
   ```bash
   git clone "[https://github.com/m1cr0-dot/Immo-35-estimator-Machine-Learning.git](https://github.com/m1cr0-dot/Immo-35-estimator-Machine-Learning.git)"
   cd Immo-35-estimator-Machine-Learning

2.  **Install dependencies :**
    ```bash
    pip install -r requirements.txt
    ```

3.  **Run the app :**
    ```bash
    streamlit run app.py
    ```

## 👤 Author

Project created by **Mateo CUNHA** as part of a personal Data Science Portfolio.
