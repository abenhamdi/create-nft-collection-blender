# 🖼️ Create NFT Collection with Blender + Python

Un projet qui permet de générer automatiquement une collection NFT unique à l’aide de Blender (modélisation 3D) et Python (automatisation). Ce script automatise la création, le rendu et l'export d'images NFT en 3D.

---

## 🎯 Objectif

* Générer des images NFT 3D en combinant des traits/modèles Blender.
* Automatiser le rendu avec des scripts Python directement dans Blender.
* Générer des métadonnées associées pour chaque NFT.
* Préparer une collection complète prête à être mintée sur une blockchain.

---

## 🧰 Technologies utilisées

* **Blender** – logiciel de modélisation 3D open source
* **Python 3.x** – scripting et automatisation
* `bpy` – Blender Python API

---

## 📁 Structure du projet

```
create-nft-collection-blender/
│
├── assets/                       # Répertoire contenant les objets et éléments 3D
│
├── blender_scripts/
│   ├── generate_nfts.py         # Script principal de génération
│   ├── render_settings.py       # Configuration du rendu Blender
│   └── utils.py                 # Fonctions utilitaires (random, combinaison, etc.)
│
├── output/
│   ├── images/                  # Dossier de sortie pour les NFT générés
│   └── metadata/                # Métadonnées JSON pour chaque NFT
│
└── README.md
```

---

## 🚀 Lancer la génération

### 1. Préparer vos assets 3D

Ajoutez vos modèles `.blend`, objets ou groupes de calques (cheveux, yeux, accessoires...) dans le dossier `assets/`.

Organisez-les par catégorie si nécessaire (ex : `eyes/`, `hats/`, `backgrounds/`...).

### 2. Ouvrir Blender avec scripting Python

Lancez Blender depuis le terminal avec l'exécution du script :

```bash
blender --background --python blender_scripts/generate_nfts.py
```

### 3. Résultat

* Les **images rendues** sont stockées dans `output/images/`
* Les **métadonnées JSON** associées à chaque NFT sont dans `output/metadata/`

---

## 🧠 Fonctionnement

* Combine aléatoirement des éléments de différentes catégories
* Crée un personnage unique à chaque exécution
* Rend chaque image avec des angles de caméra définis
* Génère les métadonnées (`name`, `attributes`, `image`) compatibles avec les standards NFT (ex : OpenSea)

---

## 📌 Pré-requis

* [Blender](https://www.blender.org/) installé
* Python intégré dans Blender (via `bpy`)
* Connaissances de base en structure de calques Blender

---

## 📦 TODO & améliorations possibles

* Interface utilisateur graphique (via Add-on Blender)
* Support de la raréfaction (rare items, poids des traits)
* Génération de vidéos NFT (via animation)
* Intégration d’un smart contract pour mint automatique
* Hébergement IPFS ou Arweave

---

## 🎨 Exemple de rendu

*(à ajouter : captures d’écran ou exemples de NFT générés)*

---

## 👤 Auteur

* **abenhamdi** – [@abenhamdi](https://github.com/abenhamdi)

