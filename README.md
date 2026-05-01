# 🧠 Deep Learning — Réseaux de Neurones & Autoencodeurs

> Quatre exercices progressifs couvrant les fondamentaux du deep learning : visualisation des activations, débruitage, CNN et autoencodeurs convolutifs.

---

##  Description

Ce Travail explore l'évolution des architectures de réseaux de neurones, du perceptron simple jusqu'aux autoencodeurs convolutifs.
Chaque partie construit sur le précédent pour comprendre comment un réseau apprend, représente et reconstruit l'information — des bases essentielles en IA appliquée à la vision et à la détection d'anomalies.

---

## 🧠 Parties

### 01 — Visualisation des Activations (Réseau Dense)
- Réseau `4 → 2 → 1` entraîné sur données personnalisées (`.npy`)
- Visualisation de l'espace latent (couche cachée 2D) à chaque epoch
- Montre comment le réseau sépare les classes au fil de l'entraînement

### 02 — Autoencodeur Dense + Débruitage (MNIST)
- Autoencodeur `784 → 32 → 784` entraîné sur MNIST
- Ajout de bruit gaussien aux images de test
- Reconstruction et comparaison : original / bruité / reconstruit

### 03 — CNN + Visualisation des Filtres (MNIST)
- Réseau CNN : `Conv2D(32) → MaxPool → Conv2D(16) → MaxPool → Dense(10)`
- Classification des chiffres MNIST avec ~99% de précision
- Visualisation des 32 filtres (couche 1) et 16 filtres (couche 2)
- Permet de comprendre ce que "voit" chaque couche convolutive

### 04 — Autoencodeur Convolutif + Débruitage
- Architecture encodeur/décodeur full-convolutif
- `Conv2D → MaxPool → Conv2D → MaxPool` / `UpSampling → Conv2D → UpSampling → Conv2D`
- Débruitage d'images MNIST avec bruit gaussien (scale=0.5)
- Affichage 3 lignes : original / bruité / reconstruit
