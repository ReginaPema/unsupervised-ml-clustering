# <img src="https://img.icons8.com/?size=50&id=wBVr33b_6fzI&format=png&color=000000" align="center"/> Unsupervised Machine Learning: Clustering & Dimensionality Reduction
### Aprendizaje No Supervisado: Clustering y Reducción de Dimensiones

> **EN** · Four notebooks covering the core unsupervised learning techniques: Hierarchical Clustering, K-Means, PCA, and KNN similarity search with Market Basket Analysis. Each notebook uses a real-world dataset and includes full exploratory analysis, model validation, and strategic conclusions.
>
> **ES** · Cuatro notebooks que cubren las técnicas centrales de aprendizaje no supervisado: Clustering Jerárquico, K-Means, PCA y búsqueda de similitud con KNN más análisis de canasta de compras. Cada notebook usa un dataset real e incluye análisis exploratorio completo, validación del modelo y conclusiones estratégicas.

---

## <img src="https://img.icons8.com/?size=40&id=80454&format=png&color=000000" align="center"/> Notebooks

### 01 · Hierarchical Clustering: Amazon Customer Recommendation System
**Dataset:** Amazon customer ratings | 100 customers × 9 product dimensions  
**Techniques:** Agglomerative Clustering · Ward Linkage · Dendrogram · PCA 2D · Recommendation Engine

- Applied Ward hierarchical clustering to segment 100 Amazon customers across 9 product categories
- Selected k=4 clusters from dendrogram analysis
- Built a personalized recommendation function: finds a customer's cluster and suggests products based on peer purchasing patterns
- Visualized cluster profiles and 2D PCA projection

---

### 02 · K-Means Clustering: Iris Dataset
**Dataset:** Iris | 150 observations × 4 features (public URL)  
**Techniques:** K-Means · Elbow Method · Silhouette Score · PCA · Adjusted Rand Index

- Compared two K-Means approaches: raw features vs PCA-reduced features
- Selected k=3 through Elbow Method and Silhouette Score
- Evaluated segmentation quality against ground-truth species labels using Adjusted Rand Index
- Visualized cluster separation in 2D PCA space

---

### 03 · PCA: Principal Component Analysis on Iris
**Dataset:** Iris | 150 observations × 4 features (public URL)  
**Techniques:** PCA · Scree Plot · Loadings · Biplot · Variance Explained

- Reduced 4 features to 2 principal components explaining 95.8% of total variance
  - PC1: 72.96% — overall size dimension (sepal + petal)
  - PC2: 22.85% — shape contrast (sepal width vs petal)
- Produced full biplot: scree plot, loadings heatmap, observations scatter, factors map, and combined biplot
- Identified petal length and petal width as the most discriminating variables

---

### 04 · KNN Similarity Search & Market Basket Analysis
**Datasets:** Wine (178 wines × 13 features) · Synthetic grocery basket (11 transactions)  
**Techniques:** KNN · NearestNeighbors · Apriori · Association Rules · Support · Confidence · Lift

**Problem 1: KNN Wine:**
- Found the 5 most chemically similar wines to a custom query point using Euclidean distance in standardized feature space

**Problem 2: Market Basket:**
- Applied Apriori to 11 grocery transactions and extracted association rules
- Key rule: Butter → Tomatoes (Confidence: 83%, Lift: 1.53)
- Identified cross-selling opportunities based on support, confidence and lift metrics

---

## <img src="https://img.icons8.com/?size=40&id=80431&format=png&color=000000" align="center"/> Tools / Herramientas

![Python](https://img.shields.io/badge/Python-8B9E8B?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-6B7F6B?style=flat&logo=pandas&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/scikit--learn-B8A9C9?style=flat&logo=scikit-learn&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-7A9E9F?style=flat&logo=scipy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=flat)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=flat)
![Jupyter](https://img.shields.io/badge/Jupyter-C4A882?style=flat&logo=jupyter&logoColor=white)

---

### <img src="https://img.icons8.com/?size=40&id=sM98nozehZSG&format=png&color=000000" align="center"/> Data Sources / Fuentes de Datos

| Notebook | Dataset | Source |
|---|---|---|
| 01 | Amazon customer ratings | [JoseRaulCastro/EBAC (GitHub)](https://github.com/JoseRaulCastro/EBAC/raw/main/Amazon.xlsx) — loaded automatically |
| 02 & 03 | Iris | [netj/8836201 (GitHub Gist)](https://gist.github.com/netj/8836201) — loaded automatically |
| 04 | Wine clustering | [Kaggle: harrywang/wine-dataset-for-clustering](https://www.kaggle.com/datasets/harrywang/wine-dataset-for-clustering) — placed in `data/` |
| 04 | Grocery basket | Defined inline — no file needed |

---

## <img src="https://img.icons8.com/?size=40&id=80358&format=png&color=000000" align="center"/> Related Projects / Proyectos Relacionados

These notebooks complement the applied clustering project:

| Project | Description |
|---|---|
| [kmeans-vanish-segmentation](https://github.com/ReginaPema/kmeans-vanish-segmentation) | Vanish brand market segmentation: K-Means on 28,377 real retail transactions |

---

## <img src="https://img.icons8.com/?size=40&id=PhymLYNNjf3I&format=png&color=000000" align="center"/> Repository Structure / Estructura

```
unsupervised-ml-clustering/
├── notebook/
│   └── 01_hierarchical_clustering_amazon.ipynb
│   └── 02_kmeans_iris.ipynb
│   └── 03_pca_iris.ipynb
│   └── 04_knn_market_basket.ipynb
├── data/
│   └── wine-clustering.csv     ← required for notebook 04
└── README.md
```

---

*Project developed as part of the Data Scientist Certificate · 
Proyecto desarrollado como parte del certificado Científico de Datos — EBAC (2026)* <img src="https://img.icons8.com/?size=35&id=FgMs84V9yrMV&format=png&color=000000" align="center"/>
