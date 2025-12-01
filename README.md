# Geometric Deep Learning Transformer for Skeleton-Based Action Recognition

📄 **Article Accepté** | Computer Vision Research

Modèle amélioré de Geometric Deep Learning Transformer (GDT) pour la reconnaissance d'actions humaines à partir de séquences de squelettes 3D. Ce projet intègre des modules Transformer et une couche de manifold learning pour capturer les dynamiques spatio-temporelles complexes des mouvements humains.

## 🎯 Objectif

Développer un modèle de deep learning capable de reconnaître avec précision des actions humaines à partir de données de squelettes 3D en exploitant la géométrie non-euclidienne et les relations spatio-temporelles des articulations corporelles.

## 🔄 Architecture du Système

### 1. Modélisation Sphérique
Représentation des squelettes comme éléments sur une sphère unitaire (manifold riemannien). Cette approche permet de capturer la structure géométrique intrinsèque des données tout en éliminant les variations d'échelle.

### 2. Inverse Exponential Map
Projection des données depuis le manifold riemannien vers l'espace tangent euclidien. Cette transformation permet d'appliquer des opérations de deep learning standard tout en préservant les propriétés géométriques des données.

### 3. Spatial Transformer Attention
Module d'auto-attention spatiale qui capture les corrélations entre les différentes articulations du corps à chaque instant.

### 4. Temporal Transformer Attention
Module d'auto-attention temporelle qui analyse l'évolution de chaque articulation à travers le temps.

### 5. Manifold Learning Layer
Couche innovante qui exploite la structure géométrique complexe des données squelettes. Cette couche améliore significativement la capacité du modèle à comprendre les patterns structurels.

### 6. Classification
Tête MLP (Multi-Layer Perceptron) finale qui transforme les features extraites en prédictions de classes d'actions.

## 🛠️ Technologies et Modèles

- **Architecture**: Transformer-based Networks (Spatial, Temporal, Spatio-Temporal)
- **Geometric Deep Learning**: Riemannian Manifolds, Spherical Modeling
- **Attention Mechanism**: Multi-Head Self-Attention (MHSA)
- **Deep Learning Framework**: PyTorch
- **Computer Vision**: 3D Skeleton Sequence Processing

## 📊 Évaluation

### Datasets Utilisés

**NTU RGB+D**
- 56,000 clips vidéo
- 60 classes d'actions
- Protocoles: Cross-Subject, Cross-View

**NTU RGB+D 120**
- 114,000+ échantillons vidéo
- 120 classes d'actions
- Protocoles: Cross-Subject, Cross-Setup

**Les résultats détaillés et les comparaisons avec l'état de l'art sont disponibles dans l'article.**

## ✨ Contributions Principales

### 1. Intégration du Manifold Learning
Première intégration d'une couche de manifold learning dans une architecture Transformer pour la reconnaissance d'actions basées sur squelettes.

### 2. Architecture Spatio-Temporelle Unifiée
Développement d'un framework Transformer unifié optimisé spécifiquement pour les séquences de squelettes.

### 3. Performances State-of-the-Art
Résultats surpassant les approches existantes sur les benchmarks NTU RGB+D et NTU RGB+D 120.

## 🎓 Applications

- Surveillance Vidéo
- Interaction Homme-Machine
- Santé et Réhabilitation
- Réalité Virtuelle
- Analyse Sportive



---

*Geometric Deep Learning research for 3D human action recognition using Transformer architectures and manifold learning*
