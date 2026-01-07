# Projet : Réduction de dimensionnalité et régression sur données agricoles

Ce projet propose une analyse complète de données agricoles à l’aide de l’Analyse en Composantes Principales (ACP) et de la régression linéaire multivariée, avec prise en compte de l’accélération GPU si disponible.

## Objectifs

- Nettoyer et préparer des données agricoles issues de plusieurs fichiers CSV
- Réduire la dimensionnalité par ACP
- Prédire plusieurs variables cibles par régression linéaire multivariée
- Interpréter les résultats et l’importance des variables
- Accélérer les calculs via GPU (PyTorch, cuML, ou Google Colab)

## Structure du notebook

1. **Préparation des données** : chargement, nettoyage, sélection des variables explicatives et cibles
2. **Standardisation** : centrage-réduction des variables numériques
3. **ACP** : réduction de dimension, visualisation de la variance expliquée, projection
4. **Régression linéaire** : entraînement sur les composantes principales, prédiction
5. **Évaluation** : métriques R² et RMSE, analyse des coefficients
6. **Accélération GPU** : exemples avec cuML et PyTorch, instructions pour Google Colab

## Installation et utilisation

1. **Créer un environnement virtuel (recommandé)**
   Ouvrez un terminal dans le dossier du projet et tapez :

```bash
python -m venv venv
```

Activez l’environnement :

- Sous Windows :
  ```bash
  venv\Scripts\activate
  ```
- Sous Linux/Mac :
  ```bash
  source venv/bin/activate
  ```

2. **Installer les dépendances**
   Assurez-vous d’avoir un fichier `requirements.txt` dans le dossier du projet. Installez les dépendances avec :

```bash
pip install -r requirements.txt
```

3. **Lancer le notebook**
   Ouvrez le fichier `exam.ipynb` avec Jupyter Notebook ou VS Code, puis exécutez les cellules étape par étape.

4. **Données**
   Placez vos fichiers CSV dans le dossier `data` avant de lancer l’analyse.

5. **Accélération GPU (optionnel)**
   Suivez les instructions du notebook pour activer le GPU sur Google Colab ou installez les bibliothèques compatibles GPU si vous avez une carte NVIDIA.

## Utilisation

1. Placez vos fichiers CSV dans le dossier `data/`.
2. Ouvrez le notebook `exam.ipynb`.
3. Exécutez chaque cellule étape par étape.
4. Pour profiter du GPU :
   - Sur Google Colab : importez le notebook, activez le GPU, installez cuML/cupy/torch.
   - En local : installez PyTorch (CPU ou GPU selon votre matériel).

## Dépendances principales

- Python ≥ 3.13
- pandas, numpy, matplotlib, seaborn
- scikit-learn
- torch (PyTorch)
- cupy, cuml (optionnel, pour GPU)

## Accélération GPU

- **PyTorch** : automatique si GPU compatible CUDA
- **cuML** : nécessite une carte NVIDIA et drivers CUDA
- **Google Colab** : instructions dans le notebook pour activer le GPU

## Interprétation

Le notebook fournit des visualisations et des analyses pour comprendre l’impact des variables sur les prédictions et la qualité du modèle.

## Auteur

- Projet réalisé dans le cadre d’un exercice de data science
- mail :**maximeatsoudegbovi@gmail.com**
