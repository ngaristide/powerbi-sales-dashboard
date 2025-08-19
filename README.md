# 📊 Power BI Dashboard – Suivi des Ventes & Commandes Annulées

## 🚀 Contexte du projet
Ce projet a pour objectif de construire un **dashboard interactif sous Power BI** permettant d’analyser les ventes, de suivre les performances commerciales et d’explorer les **commandes annulées**.  
Il met en avant les bonnes pratiques de **préparation des données, modélisation et visualisation BI**.

---

## 📂 Contenu du dépôt
- `sales_2.csv` → Dataset brut utilisé pour l’analyse  
- `Dashboard_Sales.pbix` → Fichier Power BI contenant le rapport final  
- `README.md` → Documentation du projet  

---

## 🔧 Étapes du projet

### 1. Préparation & Nettoyage des données
- Import du fichier `sales_2.csv` dans **Power Query**  
- Vérification des types de données et de leur qualité  
- Renommage des colonnes pour plus de clarté  

### 2. Normalisation & Modélisation
- Création de tables de référence : **Clients, Produits, Régions**  
- Construction de la table de faits **Ventes**  
- Mise en place d’un **modèle relationnel** clair  
- Vérification des relations automatiques et création manuelle si nécessaire  

### 3. Mesures DAX
- `Total ventes = SUM(Ventes[Prix total])`  
- `Nombre de commandes = DISTINCTCOUNT(Ventes[Id commande])`  
- `Quantité vendue = SUM(Ventes[Quantité])`  
- `Commande moyenne = DIVIDE([Total ventes], [Nombre de commandes])`  
- Mesures spécifiques aux commandes annulées (% et montants)  

### 4. Visualisations
- **Onglet 1 – Suivi des ventes**
  - KPI : ventes totales, nombre de commandes, quantités, commande moyenne  
  - Courbe d’évolution des ventes dans le temps  
  - Répartition du CA par **région** et **catégorie produit**  
  - Tableau détaillé des commandes  

- **Onglet 2 – Commandes annulées**
  - KPI dédiés (montant, nombre et % d’annulations)  
  - Courbe d’évolution du taux d’annulation  
  - Histogrammes, treemap et ruban par produit  

### 5. Fonctionnalités avancées
- Thème personnalisé (Loomy Lime Theme)  
- Menu de navigation avec icônes  
- **Info-bulles dynamiques** (tooltips)  
- **Signets (bookmarks)** pour filtres rapides  
- **Row-Level Security (RLS)** : gestion d’accès par société ou par région  
- Version mobile optimisée  
- Publication sur **Power BI Service**  

---

## 📸 Aperçu du dashboard
*(Ajouter ici vos captures d’écran du rapport Power BI – par exemple onglet ventes & onglet commandes annulées)*  

### Vue d’ensemble
[modèle_onglet_suiviVentes](https://github.com/user-attachments/assets/dc90f2d1-8dd7-4230-8df0-19693174b915)


### Répartition du CA par région
[modèle_infobulle_suivi_ventes_region](https://github.com/user-attachments/assets/0bc23eb6-1d79-4e3b-86f8-e0eb86d0116c)


### Suivi des commandes annulées
[modèle_onglet_suiviCommandes_annulées](https://github.com/user-attachments/assets/d80568c5-c204-4807-979f-60d2870e0ace)

### Suivi des commandes produits
[modèle_infobulle_ruban_produits](https://github.com/user-attachments/assets/e6d8b884-d9c2-4c9e-bc8b-c063908328de)


---

## ▶️ Résultats
✅ Suivi global du chiffre d’affaires et des volumes de ventes  
✅ Analyse détaillée par client, produit et région  
✅ Monitoring spécifique des **commandes annulées**  
✅ Expérience utilisateur enrichie (navigation, filtres, info-bulles, signets)  

---

## 🧑‍💻 Auteur
👤 **Aristide Ngoualem**  
🎓 Master 2 Data Science & Stratégie – IONIS STM  
📌 Objectif : Devenir **Chief Data Officer**  
📫 Contact : ngoualemaris@gmail.com | [LinkedIn](https://www.linkedin.com/)  

