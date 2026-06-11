# 🪦 Site Vitrine - Marbrerie du Hainaut

Ce dépôt contient le code source du site vitrine de la **Marbrerie du Hainaut**, développé dans le cadre de mon stage de 2ème année d'IUT. 

Le site a pour objectif de présenter les différents services de marbrerie funéraire (création de monuments funéraires, cavurnes, pose de caveaux, et services de rénovation/réparation) avec une expérience utilisateur moderne, rapide et esthétique.

---

## 🛠️ Technologies & Stack Technique

* **Framework :** [Astro v6](https://astro.build/) (Générateur de site statique axé sur les performances et le SEO optimal).
* **Styles :** [Tailwind CSS v4](https://tailwindcss.com/) (Intégration responsive basée sur un design system moderne).
* **Composants Dynamiques :** [React](https://react.dev/) & [TypeScript](https://www.typescriptlang.org/) (Gestion du catalogue et des interactions).
* **Cartographie :** [Leaflet](https://leafletjs.com/) (Intégration d'une carte interactive et légère pour situer l'entreprise).

---

## 📂 Structure du Projet

Voici l'organisation des fichiers clés du projet :

```text
/
├── public/                     # Fichiers statiques (favicon, images, etc.)
├── src/
│   ├── assets/                 # Ressources graphiques et illustrations
│   ├── components/             # Composants réutilisables du site
│   │   ├── Navbar.astro        # Barre de navigation
│   │   ├── Footer.astro        # Pied de page
│   │   ├── Location.astro      # Bloc adresse & Carte interactive (Leaflet)
│   │   ├── ContactForm.astro   # Formulaire de contact / Devis
│   │   └── *Gallery.astro      # Galeries photos interactives par service
│   ├── layouts/
│   │   └── Layout.astro        # Layout HTML de base (metadonnées, SEO, Google Fonts)
│   ├── pages/                  # Pages du site (générant automatiquement les routes)
│   │   ├── index.astro         # Page d'accueil
│   │   ├── catalogue.astro     # Catalogue de monuments funéraires
│   │   ├── caveau.astro        # Section construction de caveaux
│   │   ├── cavurne.astro       # Section monuments cinéraires (cavurnes)
│   │   ├── reparation.astro    # Section entretien et rénovation
│   │   ├── contact.astro       # Page de contact
│   │   └── mentions-legales.astro
│   └── styles/
│       └── global.css          # Styles globaux (import Tailwind + variables de thème)
├── astro.config.mjs            # Configuration d'Astro et de ses intégrations
└── package.json                # Dépendances et scripts npm
```

---

## 🚀 Lancer le projet sur un nouveau PC

Suivez ces étapes simples pour faire fonctionner le site localement :

### 1. Prérequis
Assurez-vous que **Node.js** (version `>= 22.12.0` recommandée) est installé sur votre machine. 
Vous pouvez le télécharger sur [nodejs.org](https://nodejs.org/).

### 2. Cloner le dépôt
Récupérez le projet depuis GitHub :
```bash
git clone <URL_DU_DEPOT_GITHUB>
cd marbrerie_du_hainaut
```

### 3. Installer les dépendances
Installez les bibliothèques et modules nécessaires à l'aide de npm :
```bash
npm install
```

### 4. Lancer le serveur de développement
Démarrez le serveur local pour visualiser et modifier le site en temps réel :
```bash
npm run dev
```
Une fois la commande exécutée, ouvrez votre navigateur et accédez à l'adresse suivante :  
👉 **[http://localhost:4321](http://localhost:4321)**

### 5. Compiler pour la production (Optionnel)
Pour générer les fichiers HTML/CSS statiques optimisés (distribuables) :
```bash
npm run build
```
Les fichiers générés se trouveront dans le dossier `/dist/`. Pour tester ce build de production localement :
```bash
npm run preview
```
