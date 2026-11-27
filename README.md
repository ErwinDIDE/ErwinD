# Erwin DIDE — Recherche un stage de fin d'études

### Étudiant en dernière année de Master spécialisation Data

Bienvenue sur mon profil GitHub ! Je suis passionné par l'ingénierie des données, de la construction des systèmes pour collecter et traiter des données qui sont utilisées pour relever des décisions commerciales à l'orchestration de pipelines complexes et le MLOps.

<div align="center">
  <img src="profil.jpeg" alt="Erwin DIDE" width="160" style="border-radius: 50%; width: 160px; height: 160px; object-fit: cover;" />
  <h1>Erwin DIDE</h1>
  <p><b>Étudiant en dernière année de Master</b></p>
</div>

---

## Stack Technique & Compétences

| Domaine | Technologies & Outils |
| :--- | :--- |
| **Bases de données** | PostgreSQL, MySQL, DuckDB, MongoDB, Oracle |
| **Orchestration & ETL/ELT** | Airflow, Dagster, dbt, Talend |
| **Cloud & Storage** | GCP (BigQuery, Vertex AI), Distributed Systems (Hadoop, Kafka) |
| **MLOps & CI/CD** | MLflow, W&B, Docker, Kubernetes, GitHub Actions, GitLab CI, DVC |
| **Langages** | Python, SQL, Java, C |
| **Data Viz & BI** | Tableau, Power BI, Metabase, Streamlit |

---

## 📌 Projets à la une

### <a href="https://github.com/ErwinDIDE/projet-sql-data-warehouse"><img src="https://cdn.jsdelivr.net/npm/lucide-static@latest/icons/link-2.svg" width="20" height="20" alt="Icône de lien" /></a> Projet DataWarehouse et Analytics

#### <a href="#-architecture-des-données"><img src="https://cdn.jsdelivr.net/npm/lucide-static@latest/icons/link-2.svg" width="16" height="16" alt="Icône de lien" /></a> 🏗️ Architecture des données

L'architecture des données de ce projet suit une **architecture Médaillon** articulée autour des couches **Bronze**, **Silver** et **Gold** :

<p align="center">
  <img src="architecture.drawio.png" alt="Architecture des données" width="100%" />
</p>

1. **Couche Bronze :** Stocke les données brutes telles quelles depuis les systèmes sources. Les données sont ingérées à partir de fichiers CSV vers une base de données SQL Server.
2. **Couche Silver :** Comprend les processus de nettoyage, de standardisation et de normalisation afin de préparer les données pour l'analyse.
3. **Couche Gold :** Héberge les données prêtes pour le métier, modélisées selon un schéma en étoile (*star schema*) requis pour le reporting et l'analytique.

#### <a href="#-modèle-dintégration"><img src="https://cdn.jsdelivr.net/npm/lucide-static@latest/icons/link-2.svg" width="16" height="16" alt="Icône de lien" /></a> 🔗 Modèle d'intégration

Le diagramme suivant présente le modèle d'intégration des données et les relations entre les tables :

<p align="center">
  <img src="integration_model.drawio.png" alt="Modèle d'intégration des données" width="100%" />
</p>

---

### 📊 [Dashboards & Analytics (Ventes & CRM)](https://github.com/ErwinDIDE)
> **Stack :** `Tableau`
- Conception de tableaux de bord interactifs pour l'analyse de performances multi-annuelles et l'aide à la décision business.
- *Découvrez mon dashboard interactif en ligne sur [Mon profil Tableau Public](https://public.tableau.com/app/profile/erwin.dide/vizzes).*

<section id="tableau-dashboard" style="margin: 40px 0;">
  <h2>📊 Tableau de bord interactif – Analyse des Ventes Multi-Années</h2>
  <p>Explorez les KPIs, filtrez par région ou catégorie de produits directement ci-dessous :</p>

  <div style="position: relative; width: 100%; height: 750px; border-radius: 8px; overflow: hidden; box-shadow: 0 4px 12px rgba(0,0,0,0.15);">
    <iframe 
      src="https://public.tableau.com/views/Projet_Dashboard_Ventes_Multi_Annees/SalesDashboard?:showVizHome=no&:embed=true" 
      width="100%" 
      height="100%" 
      style="border: none;">
    </iframe>
  </div>

  <p style="font-size: 0.9em; text-align: center; margin-top: 10px;">
    <i>Problème d'affichage ? <a href="https://public.tableau.com/views/Projet_Dashboard_Ventes_Multi_Annees/SalesDashboard" target="_blank">Ouvrir directement sur Tableau Public ↗</a></i>
  </p>
</section>

---

### 📊 [Dashboards & Analytics - Power BI](https://github.com/ErwinDIDE)
> **Stack :** `Power BI` • `DAX` • `Modélisation de Données`
- Modélisation de données analytiques, création de mesures DAX et conception de rapports visuels interactifs.
- Analyse des ventes, suivi du volume de commandes et segmentation des clients.

#### 📊 Tableau de bord – Sales Dashboard 2026 (Power BI)

<p align="center">
  <img src="Dashboard.jpg" alt="Sales Dashboard 2026" width="100%" />
  <br />
  <i>🛠️ Modélisation en étoile & mesures DAX développées sous Power BI Desktop</i>
</p>

---

### 📊 [E-Commerce Data Pipeline & Dashboard](https://github.com/ErwinDIDE)
> **Stack :** `Python` • `Streamlit` • `Dagster` • `dbt` • `Docker` • `REST API`
- Conception d'un pipeline ELT complet et d'un dashboard analytique pour le suivi de performances d'un site e-commerce :
  - **Ingestion & Extraction :** Collecte des données brutes (Produits, Utilisateurs, Commandes) depuis l'API *DummyJSON*.
  - **Orchestration :** Gestion du workflow et matérialisation des *Data Assets* avec **Dagster**.
  - **Modélisation & Data Warehousing :** Création des tables de faits et de dimensions (schéma en étoile) avec **dbt**.
  - **Visualisation & Conteneurisation :** Application interactive **Streamlit** pour piloter les KPIs analytiques, conteneurisée sous **Docker**.

#### 🏗️ Architecture & Modélisation du Pipeline

<table>
  <tr>
    <td align="center" width="50%">
      <img src="DAG_Dagster.png" alt="Dagster Assets Lineage" width="100%" />
      <br />
      <i>Graphe d'orchestration & dépendances des Data Assets (Dagster)</i>
    </td>
    <td align="center" width="50%">
      <img src="LINEARGRAPH.png" alt="Star Schema dbt DuckDB" width="100%" />
      <br />
      <i>Modélisation décisionnelle en étoile - Star Schema (dbt / DuckDB)</i>
    </td>
  </tr>
</table>

<section id="streamlit-dashboard" style="margin: 40px 0;">
  <h2>📊 Application – E-Commerce Analytics (Streamlit)</h2>
  <p>Explorez le tableau de bord alimenté par le pipeline Dagster & dbt :</p>

  <div style="position: relative; width: 100%; height: 750px; border-radius: 8px; overflow: hidden; box-shadow: 0 4px 12px rgba(0,0,0,0.15);">
    <iframe 
      src="https://data-processingapp.streamlit.app/?embed=true" 
      width="100%" 
      height="100%" 
      style="border: none;">
    </iframe>
  </div>

  <p style="font-size: 0.9em; text-align: center; margin-top: 10px;">
    <i>Problème d'affichage ? <a href="https://data-processingapp.streamlit.app" target="_blank">Ouvrir l'application dans un nouvel onglet ↗</a></i>
  </p>
</section>

---

### 🚕 [Pipeline de Données Scalable (Taxi & Météo)](https://github.com/ErwinDIDE)
> **Stack :** `Spark` • `Flink` • `dbt` • `Airflow` • `Docker`
- Conception d'une architecture modulaire capable d'ingérer, stocker et transformer des données de trajets de taxis en temps réel croisées avec des conditions météo.
- Modélisation de données analytiques et orchestration bout en bout du pipeline.

---

### 💳 [Plateforme MLOps - Détection de Fraude Bancaire](https://github.com/ErwinDIDE)
> **Stack :** `Python` • `FastAPI` • `MLflow` • `W&B` • `XGBoost`
- Entraînement et optimisation d'un modèle de classification XGBoost sur des données Kaggle pour maximiser le rappel et la précision.
- Mise en place d'une API de prédiction performante via **FastAPI**.
- Tracking des expériences, versioning des modèles et suivi des métriques en temps réel sur **MLflow** & **W&B**.

---

## 🎓 Formation

- **Master d'Ingénierie — Spécialisation Data** | *SUPINFO* (2025 - 2027)
  - *Data Viz, Machine Learning (Vision, Classification, Réseaux de neurones), Admin DB & Systèmes Distribués.*

---

## 📬 Me contacter

- **📍 Localisation :** Rouen, France
- **📧 Email :** [didymedide0808@gmail.com](mailto:didymedide0808@gmail.com)
- **💼 LinkedIn :** [LinkedIn - Erwin DIDE](https://linkedin.com/in/erwin-dide)
- **📊 Tableau Public :** [Profil Tableau Public](https://public.tableau.com/app/profile/erwin.dide/vizzes)
