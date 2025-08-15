
## 📌 `SECU_DATA-MAIN` — Confidentialité des données avec IA & CKKS (Flask + TenSEAL)

> 🔒 Projet d'application web autour de la **confidentialité des données** via le **chiffrement homomorphe** (CKKS), combiné à des modèles de **régression linéaire** et **logistique** intégrés dans une interface Flask.

---

### 📁 Structure du projet

```
SECU_DATA-MAIN/
├── src/                        # Code métier (modèles ML)
│   ├── logistic.py            # Régression logistique (TenSEAL)
│   └── regression_line.py     # Régression linéaire (TenSEAL)
│
├── static/                    # Fichiers statiques (data, CSS)
│   ├── data/                  # Données pour les tests
│   ├── data_linear/           # Données spécifiques à la régression linéaire
│   ├── dist/output.css        # CSS généré
│   └── src/input.css          # Fichier CSS source
│
├── templates/                 # Templates HTML Flask
│   ├── base.html
│   ├── index.html
│   ├── iris.html
│   └── logistic_base.html
│
├── app.py                     # Point d'entrée de l'application Flask (à ajouter)
├── requirements.txt           # Dépendances du projet (à générer)
└── README.md                  # Description du projet
```

---

### 🚀 Lancer l'application

1. **Créer un environnement virtuel** :

```bash
python -m venv venv
source venv/bin/activate       # Linux / Mac
venv\Scripts\activate          # Windows
```

2. **Installer les dépendances** :


> manuellement :

```bash
pip install flask scikit-learn matplotlib pandas numpy torch tenseal
```

3. **Lancer l’application Flask** :

```bash
python app.py
```

Puis ouvrir dans votre navigateur :
📍 `http://127.0.0.1:5000/`

---

### 📊 Fonctionnalités

* 🔒 **Traitement sécurisé de données sensibles** grâce au chiffrement **CKKS (TenSEAL)**.
* 📈 Modèles IA intégrés :

  * Régression linéaire
  * Régression logistique
* 🌐 Interface web Flask avec rendu HTML via `render_template`.
* 📂 Affichage de fichiers, résultats, graphiques (Matplotlib).

---

### 🧠 Objectif académique

Ce projet a été développé dans le cadre d’un **mémoire de recherche de Master** sur le thème :

> **Étude du cryptosystème CKKS pour la confidentialité des données dans les modèles d’apprentissage automatique : cas de la régression linéaire et de la régression logistique**

---

### 🙏 Remerciements

Ce projet s’inscrit dans un parcours de recherche mêlant **cryptographie homomorphe** et **intelligence artificielle**, avec le soutien du :

* **Laboratoire d’Algèbre, de Cryptologie et de Géométrie Algébrique – UCAD**
* **Orange Digital Center** pour le renforcement en IA pratique


### 📘 Licence

Ce projet est partagé à des fins **éducatives et de recherche**. Libre d’usage académique.
