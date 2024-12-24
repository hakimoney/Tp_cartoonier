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
  - La visualisation 3D des caractéristiques spatiales
  - Diviser le jeu de données en ensembles d'entraînement et de test.
  - Prétraitement et redimensionnement des données(**images(100, 128, 128, 3)**) pour l'entraînement en TensorFlow

---

### 2. **Entraîner le GAN Pix2Pix**
- **Objectif** : Mapper des images réelles vers leurs versions cartoonisées.
- **Étapes** :
  - Chargement des images et définition du modèle discriminant
  - Définition d'un modèle générateur U-Net pour la conversion d'images avec blocs d'encodage et de décodage
  Définition du Modèle GAN combiné pour l'entraînement Pix2Pix
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
  https://machinelearningmastery.com/how-to-develop-a-pix2pix-gan-for-image-to-image-translation/

---

## Prérequis
absl-py==2.1.0
astunparse==1.6.3
certifi==2024.12.14
charset-normalizer==3.4.0
contourpy==1.3.1
cycler==0.12.1
flatbuffers==24.12.23
fonttools==4.55.3
gast==0.6.0
google-pasta==0.2.0
grpcio==1.68.1
h5py==3.12.1
idna==3.10
keras==3.7.0
kiwisolver==1.4.7
libclang==18.1.1
Markdown==3.7
markdown-it-py==3.0.0
MarkupSafe==3.0.2
matplotlib==3.10.0
mdurl==0.1.2
ml-dtypes==0.4.1
namex==0.0.8
numpy==2.0.2
opencv-python==4.10.0.84
opt_einsum==3.4.0
optree==0.13.1
packaging==24.2
pillow==11.0.0
protobuf==5.29.2
Pygments==2.18.0
pyparsing==3.2.0
python-dateutil==2.9.0.post0
requests==2.32.3
rich==13.9.4
setuptools==75.6.0
six==1.17.0
tensorboard==2.18.0
tensorboard-data-server==0.7.2
tensorflow==2.18.0
tensorflow_intel==2.18.0
termcolor==2.5.0
typing_extensions==4.12.2
urllib3==2.3.0
Werkzeug==3.1.3
wheel==0.45.1
wrapt==1.17.0


---

## Installation
Telecharger le projet: 
https://e.pcloud.link/publink/show?code=kZtM9wZBdc05GD2zHLCtQSBODVgGhT2RaAV

