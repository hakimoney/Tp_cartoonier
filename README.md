# Projet Final : Cartooniser des Images avec un GAN Pix2Pix

## Description
Ce projet consiste à créer un pipeline complet pour transformer des images réelles en leur version cartoonisée à l'aide opencv et  d'un GAN Pix2Pix (GAN conditionnel). Le projet comprend la création d'un jeu de données appariées, l'entraînement du modèle Pix2Pix et la validation des résultats sur des images et vidéos.

---

## Étapes du Projet

### 1. **Créer le Jeu de Données**
- **Objectif** : Collecter des données appariées (images réelles et leurs équivalents cartoonisés).
- **Étapes** :
  - Collecter des jeux de données publics (visages, animaux, nature, routes, etc.).
  - Développer un script avec OpenCV pour styliser les images (transformer chaque image dans un style cartoon).
  - Utiliser des blogs et ressources sur le rendu non photoréaliste pour améliorer le style cartoon.
  - Diviser le jeu de données en ensembles d'entraînement et de test.

---

### 2. **Entraîner le GAN Pix2Pix**
- **Objectif** : Mapper des images réelles vers leurs versions cartoonisées.
- **Étapes** :
  - Implémenter un GAN Pix2Pix avec un générateur et un discriminateur.
  - Entraîner le modèle sur les images appariées.
  - Valider les résultats sur l'ensemble de test et sur de nouvelles images réelles.
  - Afficher une démo des résultats sur une vidéo.

---

## Détails Techniques

### **Fonctionnement du GAN**
- **Générateur** :
  - Prend en entrée une image réelle et produit une version cartoonisée.
- **Discriminateur** :
  - Tente de distinguer les images cartoon générées des images cartoon réelles.
- **Fonctions de Perte** :
  - **Perte antagoniste** : Entraîne le générateur à produire des images réalistes.
  - **Perte L1** : Assure la similitude entre les images générées et les images cartoon réelles.

### **Ressources Utilisées**
- Frameworks : TensorFlow, Keras, OpenCV.
- Références :
  - Blogs sur le rendu non photoréaliste et le transfert de style.
  - Tutoriels sur Pix2Pix et les GAN conditionnels.

---

## Prérequis
- **Python 3.x**
- **TensorFlow** (compatible avec GPU pour accélérer l'entraînement)
- **Numpy**
- **OpenCV**

---

## Installation


