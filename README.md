**Name** : **Prudhvi VVR Ajay Sreenivas**
**Roll no.** : **DA25M023**

# 🧬 Dimensionality Reduction on Gene Expression Data

*Exploring Global vs. Local Structure with Isomap and t-SNE*

---

## 📖 Overview

This repository contains a Jupyter Notebook (`main.ipynb`) that applies **manifold learning techniques** to high-dimensional **gene expression data**. The goal is to:

* Reduce data to **2D embeddings** for visualization.
* Compare **Isomap** (global structure preserving) vs **t-SNE** (local structure preserving).
* Understand the **geometry of the underlying data manifold** and its impact on classification difficulty.

---

## ⚙️ Techniques Used

* **Data Scaling** → Features are normalized before dimensionality reduction.
* **Isomap** → Preserves **global geometry** using geodesic distances.
* **t-SNE** → Preserves **local neighborhood structure** via probabilistic embeddings.
* **Visualization** → Scatter plots of embeddings colored by class labels.
* **Analysis** → Discussion of manifold curvature and implications for classification.

---

## 📊 Results

### 🔹 Isomap (Global Structure)

* Produces a **continuous embedding**, spreading out samples smoothly.
* Captures **overall relationships** between samples across the dataset.
* Reveals that the gene expression manifold is **highly curved**.

### 🔹 t-SNE (Local Structure)

* Produces **clustered embeddings** (tight groups of similar samples).
* Preserves **local neighborhoods** but distorts global distances.
* Clusters change depending on **perplexity values**.

---

## 🖼️ Visualizations

### Isomap Projection

Shows global manifold unfolding


### t-SNE Projections (Various Perplexities)

Reveals local clustering behavior

---

## 🧩 Key Insights

* **Isomap** is better for **understanding global manifold structure**.
* **t-SNE** is better for **visualizing local clusters**.
* The gene expression manifold appears **curved and complex**, making **classification harder** with simple linear models.
* Nonlinear methods (kernel SVMs, ensemble methods, deep learning) may be required to capture this complexity.

---

## 🌟 Acknowledgments

* **scikit-learn** for Isomap and t-SNE implementations.
* **matplotlib** for visualizations.
* Inspired by manifold learning applications in **computational biology**.

---

## 🔮 Future Work

* Apply **UMAP** for faster manifold learning with large-scale data.
* Explore **classification models** on reduced embeddings.
* Extend analysis to **other biological datasets**.

---
