# TP2_SQL_Chomage
TP 2- Acquisition, stockage et exploitation de données avec Google Colab et SQL

**Auteur :** Naïma Remmal - Chaimae Khaldi

**Sujet :** Analyse du taux de chômage au Maroc (selon le milieu et le sexe)  
**Source des données :** Haut-Commissariat au Plan (HCP) du Maroc  

---

## Synthèse du Projet

### 1. Présentation du Jeu de Données
Le jeu de données exploité provient du Haut-Commissariat au Plan (HCP) du Maroc. Il analyse l'évolution du taux de chômage selon le milieu de résidence (Urbain/Rural) et le sexe sur la période d'étude.

### 2. Démarche Technique
1. **Acquisition & Stockage :** Téléchargement du fichier Excel officiel du HCP et stockage dans Google Drive dans le dossier `TP_SQL_Dataset`.
2. **Exploration & Nettoyage :** Chargement dans Google Colab via Pandas, renommage explicite des colonnes et suppression des lignes parasites/vides.
3. **Modelisation SQL :** Exportation du DataFrame nettoyé dans une base de données relationnelle SQLite (`tp_sql.db`).
4. **Exploitation :** Exécution de 15 requêtes SQL progressives (sélections, filtres, agrégations, sous-requêtes) et génération de visualisations graphiques avec Seaborn.

### 3. Principaux Résultats & Conclusions
- **Disparité spatiale marquante :** Le taux de chômage moyen en milieu urbain (> 12 %) est nettement plus élevé qu'en milieu rural (~ 8 %).
- **Distribution des taux :** La majorité des observations nationales se concentrent dans un intervalle compris entre 8 % et 12 %.
- **Inégalités structurelles :** L'analyse met en évidence des écarts persistants sur le marché du travail selon le milieu de résidence.

### 4. Difficultés Rencontrées
La principale difficulté a résidé dans la restructuration préalable du fichier Excel du HCP (gestion des en-têtes complexes et alignement des colonnes) afin de garantir une conversion propre vers la base de données SQLite.
