# 🖼️ Create NFT Collection – JavaScript + Blender (Asset Generation)

Un projet JavaScript qui permet de générer automatiquement une collection NFT à partir de calques d'images, en combinant différents traits visuels (ex : fond, yeux, accessoires...) selon une logique de rareté, puis d’enregistrer les métadonnées au format JSON.

---

## 🎯 Objectif

* Générer une collection d’images NFT de manière automatisée.
* Créer les **métadonnées associées** (standard ERC-721 / OpenSea).
* Définir la **rareté** et les combinaisons possibles entre les calques.
* Exporter les images finales au format `.png` ainsi que les fichiers `.json`.

---

## 📁 Structure du projet

```
create-nft-collection-blender/
│
├── layers/                      # Dossiers contenant les calques (ex: eyes, background...)
│   ├── background/
│   ├── body/
│   └── accessories/
│
├── output/
│   ├── images/                  # Images NFT générées
│   └── metadata/                # Métadonnées JSON
│
├── config.js                    # Configuration des couches et rareté
├── index.js                     # Script principal de génération
├── package.json                 # Dépendances Node.js
└── README.md
```

---

## 🚀 Installation & exécution

### 1. Cloner le dépôt

```bash
git clone https://github.com/abenhamdi/create-nft-collection-blender.git
cd create-nft-collection-blender
```

### 2. Installer les dépendances

```bash
npm install
```

### 3. Lancer la génération de la collection NFT

```bash
node index.js
```

---

## ⚙️ Configuration

Le fichier `config.js` vous permet de :

* Définir les **couches** à superposer (ordre, rareté)
* Spécifier le **nombre total d’images** à générer
* Générer les **métadonnées JSON** compatibles avec IPFS / OpenSea
* Personnaliser les noms, attributs et formats

---

## 🧠 Fonctionnement

* Chaque image est une **combinaison aléatoire** de calques visuels.
* Les couches sont superposées dans un ordre défini (ex: background → body → eyes → accessoires).
* Une logique de **rareté pondérée** permet de générer des NFT plus ou moins rares.
* Le système vérifie qu’aucune duplication ne survient dans les images générées.
* Les **métadonnées JSON** incluent :

  * `name`, `description`, `image`, `attributes`…

---

## ✅ Résultat

* 🎨 Images générées dans `output/images/`
* 🧾 Métadonnées compatibles avec les standards NFT dans `output/metadata/`
* Prêt pour **upload sur IPFS**, **mint sur Ethereum**, ou **OpenSea**

---

## 🔧 Améliorations possibles

* Génération de GIFs ou vidéos
* Intégration avec Pinata / IPFS pour uploader automatiquement
* Interface visuelle (ex: dashboard React/Next.js)
* Gestion avancée de la raréfaction (exclusion de combinaisons)
* Export automatique vers smart contracts

---

## 📦 Dépendances clés

* `canvas` – dessin et manipulation d'images
* `fs` – gestion des fichiers
* `path` – chemins dynamiques
* `uuid` – génération d’identifiants uniques

---

## 👤 Auteur

* **abenhamdi** – [@abenhamdi](https://github.com/abenhamdi)
