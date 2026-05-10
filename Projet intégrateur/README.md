# NexaLab — Page d'accueil officielle

> Projet intégrateur · Bloc 2 · Modules 3 & 4 · Académie de Programmation IFRI L1  
> Concevoir. Structurer. Présenter comme des pros.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![Flexbox](https://img.shields.io/badge/Flexbox-00C2AA?style=flat)
![Responsive](https://img.shields.io/badge/Responsive-F0A500?style=flat)
![FontAwesome](https://img.shields.io/badge/FontAwesome-528DD7?style=flat&logo=fontawesome&logoColor=white)

---

## Table des matières

1. [Présentation du projet](#1-présentation-du-projet)
2. [Le client — NexaLab](#2-le-client--nexalab)
3. [L'équipe](#3-léquipe)
4. [Structure du dépôt](#4-structure-du-dépôt)
5. [Architecture CSS — Tableau de responsabilité](#5-architecture-css--tableau-de-responsabilité)
6. [Identité visuelle](#6-identité-visuelle)
7. [Typographie](#7-typographie)
8. [Décisions techniques](#8-décisions-techniques)
9. [Extensibilité — Ajouter une nouvelle page ou section](#9-extensibilité--ajouter-une-nouvelle-page-ou-section)
10. [Lancer le projet en local](#10-lancer-le-projet-en-local)

---

## 1. Présentation du projet

**REBUILD** est un projet intégrateur compétitif réalisé dans le cadre du Bloc 2 de l'Académie de Programmation IFRI (L1). Six groupes ont conçu et développé la page d'accueil de **NexaLab**, un laboratoire d'innovation technologique fictif ciblant les entreprises africaines.

Le projet mobilise l'ensemble des compétences acquises sur les deux premiers modules du Bloc 2 :

- Lecture et analyse de code existant
- Architecture modulaire et organisation de projet
- HTML5 sémantique et CSS3 clean code
- Responsive design (mobile, tablette, desktop)
- Versioning Git avec une branche dédiée

**Durée :** 10 jours · **Technologies :** HTML5 + CSS3 uniquement (aucun JavaScript, aucun framework)

---

## 2. Le client — NexaLab

**NexaLab** est un laboratoire fictif spécialisé dans l'innovation technologique pour les entreprises africaines. Son identité repose sur trois piliers : **modernité**, **rigueur**, **impact**.

| Attribut | Valeur |
|---|---|
| Secteur | Innovation technologique (IA, IoT, Data) |
| Cible | Directeurs d'entreprise, investisseurs, jeunes talents tech |
| Ton | Confiant, innovant, accessible |
| Identité visuelle | Sombre, épurée, technologique |
| Objectif du site | Convaincre en moins de 10 secondes |

---

## 3. L'équipe

| # | Nom complet | Rôle |
|---|---|---|
| 1 | SOZAN Euloge | |
| 2 | Iréti Folakè Thérèsa Sarah BADOU | |
| 3 | SOSSOU Merveilles de Dieu | |
| 4 | Aristote Léon Egnon HOUNTONDJI | |
| 5 | Houéfa Immaculée Christelle AHOLOU | |
| 6 | HOUENOU Adonis | |

> **Chef de projet :** SOZAN Euloge

---

## 4. Structure du dépôt

```
nexalab/
├── index.html              <- Point d'entrée unique du site
├── styles/
│   ├── base.css            <- Reset, variables CSS, typographie globale
│   ├── header.css          <- Navigation + logo
│   ├── hero.css            <- Section d'accroche principale
│   ├── about.css           <- Mission et présentation de NexaLab
│   ├── services.css        <- Expertises et domaines d'intervention
│   ├── stats.css           <- Chiffres clés
│   ├── team.css            <- Equipe ou partenaires
│   ├── testimonials.css    <- Témoignages clients
│   ├── contact.css         <- Formulaire de contact
│   └── footer.css          <- Pied de page
├── assets/
│   ├── images/             <- Visuels libres de droits (Unsplash / Pexels)
│   └── icons/              <- Icônes SVG personnalisées si nécessaire
└── README.md               <- Ce document
```

**Justification de la structure :**
Chaque fichier CSS correspond à une section précise du site. Cette séparation permet à chaque membre de l'équipe de travailler sur sa section sans conflit de merge Git. Elle facilite également la maintenance : modifier le hero ne touche jamais le footer.

Le fichier `base.css` est le socle commun — il contient les variables CSS (couleurs, polices, espacements) partagées par tous les autres fichiers via `var()`.

---

## 5. Architecture CSS — Tableau de responsabilité

| Fichier CSS | Responsabilité | Eléments gérés |
|---|---|---|
| `base.css` | Fondation globale | `:root` variables, reset CSS, styles body, import Google Fonts, classes utilitaires |
| `header.css` | Navigation principale | header, nav, logo, liens de navigation, comportement sticky |
| `hero.css` | Section d'accroche | Message principal, sous-titre, bouton CTA, fond visuel |
| `about.css` | Présentation NexaLab | Texte de mission, vision, éléments différenciants |
| `services.css` | Expertises | Cards de services, icônes Font Awesome, grille Flexbox |
| `stats.css` | Chiffres clés | Compteurs, layout horizontal, séparateurs |
| `team.css` | Equipe / Partenaires | Photos ou avatars, noms, postes, layout en grille |
| `testimonials.css` | Témoignages | Cards citations, avatars, mise en page carousel-like |
| `contact.css` | Formulaire de contact | form, input, textarea, styles des labels et bouton d'envoi |
| `footer.css` | Pied de page | Colonnes footer, liens, réseaux sociaux, copyright |

---

## 6. Identité visuelle

La palette de NexaLab repose sur deux niveaux de lecture : des fonds profonds qui installent la crédibilité technologique, et des accents chromatiques qui guident l'action et signalent l'innovation.

### Palette de couleurs

| Nom | Hex | Usage |
|---|---|---|
| **Abyss** | `#0D1B2E` | Fond principal — profondeur, ancrage |
| **Ocean** | `#152B4A` | Surfaces secondaires, cards |
| **Cobalt** | `#1B4080` | Bordures, séparateurs, éléments structurels |
| **Amber** | `#F0A500` | Accent primaire — CTA, valeur, action |
| **Teal** | `#00C2AA` | Accent secondaire — innovation, technologie |
| **Off-white** | `#E8EDF5` | Titres, textes importants |
| **Mist** | `#8BA3BC` | Corps de texte, descriptions |

```css
/* Declaration dans base.css */
:root {
  --color-abyss:    #0D1B2E;
  --color-ocean:    #152B4A;
  --color-cobalt:   #1B4080;
  --color-amber:    #F0A500;
  --color-teal:     #00C2AA;
  --color-offwhite: #E8EDF5;
  --color-mist:     #8BA3BC;
}
```

**Justification des choix :**
Le fond sombre (Abyss) installe immédiatement un registre technologique sérieux, cohérent avec l'audience cible (décideurs, investisseurs). L'Amber guide l'oeil vers les actions principales (CTA, chiffres clés) — couleur chaude sur fond froid, contraste maximum. Le Teal identifie visuellement tout ce qui touche à l'innovation et à la tech, créant un second niveau de lecture sans surcharger la hiérarchie.

---

## 7. Typographie

| Famille | Usage | Caractéristique |
|---|---|---|
| **Space Grotesk** | Titres (h1 à h3) | Géométrique, dense, autorité immédiate |
| **Plus Jakarta Sans** | Corps de texte, descriptions | Légère, fluide, lecture confortable |

```css
/* Import dans base.css */
@import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;600;700&family=Plus+Jakarta+Sans:wght@400;500;600&display=swap');

:root {
  --font-heading: 'Space Grotesk', sans-serif;
  --font-body:    'Plus Jakarta Sans', sans-serif;
}
```

**Justification :** Les deux familles partagent une construction géométrique commune qui garantit la cohérence visuelle à toutes les tailles d'écran. Space Grotesk impose une présence forte sur les grands titres ; Plus Jakarta Sans assure le confort de lecture sur de longs passages, essentiel pour les sections About, Services et Témoignages.

---

## 8. Décisions techniques

### Iconographie — Font Awesome

Les icônes sont intégrées via Font Awesome (CDN). Ce choix garantit une cohérence visuelle entre toutes les sections sans avoir à produire des SVG custom, et offre une bibliothèque complète adaptée aux thématiques tech (IA, Data, IoT).

### Layout — Flexbox principal, Grid en complément

La mise en page principale repose sur **Flexbox** pour la navigation, les cards de services, les témoignages et le formulaire. CSS Grid est utilisé en complément pour les sections à grilles symétriques (chiffres clés, équipe) où l'alignement bidimensionnel est pertinent.

### Responsive — Mobile First

Les media queries suivent une approche **mobile first** : les styles de base ciblent les petits écrans, et les breakpoints élargissent progressivement la mise en page.

```css
/* Breakpoints utilises */
/* Mobile  : 768px et moins  (defaut) */
/* Tablette: 1024px et moins          */
/* Desktop : plus de 1024px           */
```

---

## 9. Extensibilité — Ajouter une nouvelle page ou section

### Ajouter une nouvelle section à index.html

1. Créer un fichier `styles/nom-section.css`
2. Y définir les styles spécifiques à cette section en utilisant les variables de `base.css`
3. Lier ce fichier dans le `head` de `index.html` :

```html
<link rel="stylesheet" href="styles/nom-section.css">
```

4. Ajouter la section dans `index.html` avec la balise sémantique appropriée (`section`, `aside`, etc.)
5. Mettre à jour la navigation dans le `header` si nécessaire

### Ajouter une nouvelle page (ex: services.html)

1. Dupliquer `index.html` et renommer le fichier
2. Conserver les liens vers `base.css`, `header.css` et `footer.css` (communs à toutes les pages)
3. Lier uniquement les fichiers CSS spécifiques aux sections présentes sur cette page
4. Mettre à jour les liens de navigation dans le `header` pour pointer vers la nouvelle page

> Cette architecture modulaire garantit qu'aucune modification d'une section n'affecte les autres. Le projet est conçu pour grandir sans dette technique.

---

## 10. Lancer le projet en local

Aucune dépendance, aucun serveur requis.

```bash
# Cloner le depot
git clone https://github.com/Euloge-szn/BLOC_02.git

# Acceder au dossier
cd BLOC_02

# Se placer sur la bonne branche
git checkout projet-integrateur

# Ouvrir index.html dans le navigateur
# (double-clic ou clic droit > Ouvrir avec...)
```

---

<div align="center">

**Académie de Programmation · IFRI · L1 · Bloc 2**

Projet REBUILD — NexaLab · 2025

</div>
