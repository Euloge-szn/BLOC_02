# NexaLab — Page d'accueil officielle

> Projet intégrateur · Bloc 2 · Modules 3 & 4 · Académie de Programmation IFRI L1  
> Concevoir. Structurer. Présenter comme des pros.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![Flexbox](https://img.shields.io/badge/Flexbox-00C2AA?style=flat)
![Grid](https://img.shields.io/badge/CSS%20Grid-3b77df?style=flat)
![Responsive](https://img.shields.io/badge/Responsive-F0A500?style=flat)
![No JS](https://img.shields.io/badge/JavaScript-Aucun-red?style=flat)

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

| # | Nom complet | Sections réalisées |
|---|---|---|
| 1 | SOZAN Euloge | Header, Hero, À propos |
| 2 | HOUENOU Adonis | Header, Hero, À propos |
| 3 | Iréti Folakè Thérèsa Sarah BADOU | Services / Expertises, Chiffres clés |
| 4 | SOSSOU Merveilles de Dieu | Services / Expertises, Chiffres clés |
| 5 | Houéfa Immaculée Christelle AHOLOU | Formulaire de contact, Footer, Témoignages |
| 6 | Aristote Léon Egnon HOUNTONDJI | Formulaire de contact, Footer, Témoignages |
| 7 | LEFÈVRE | Formulaire de contact, Footer, Témoignages |

> **Chef de projet :** SOZAN Euloge

---

## 4. Structure du dépôt

```
Dossier-final/
├── index.html              <- Version française du site
├── index-en.html           <- Version anglaise du site
├── README.md               <- Ce document
├── CdC_Bloc2_ProjetIntegrateur.pdf  <- Cahier des charges
├── styles/
│   ├── base.css            <- Reset, variables CSS, typographie, animations
│   ├── header.css          <- Navigation + logo + sélecteur de langue
│   ├── hero.css            <- Section d'accroche (particules, courbes SVG)
│   ├── about.css           <- Mission et présentation (3 cartes ADN)
│   ├── services.css        <- Expertises (cartes avec icônes SVG)
│   ├── stats.css           <- Chiffres clés (compteurs gradient)
│   ├── team.css            <- Équipe (avatars) et partenaires
│   ├── team-membres.css    <- Photos des membres (glassmorphisme)
│   ├── testimonials.css    <- Témoignages clients (cartes citations)
│   ├── contact.css         <- Formulaire de contact (inputs premium)
│   └── footer.css          <- Pied de page (colonnes, réseaux sociaux)
├── assets/
│   ├── images/
│   │   ├── logo.png             <- Logo NexaLab
│   │   ├── about-team.webp      <- Image hero (ville africaine)
│   │   ├── hero-africa.jpg      <- Image section À propos (Afrique)
│   │   ├── member-saston.jpg    <- Photo membre
│   │   ├── member-charlie.jpg   <- Photo membre
│   │   ├── member-john.jpg      <- Photo membre
│   │   └── member-diana.jpg     <- Photo membre
│   └── icons/              <- (Réservé) Icônes SVG supplémentaires
```

**Justification de la structure :**
Chaque fichier CSS correspond à une section précise du site. Cette séparation permet à chaque membre de l'équipe de travailler sur sa section sans conflit de merge Git. Elle facilite également la maintenance : modifier le hero ne touche jamais le footer.

Le fichier `base.css` est le socle commun — il contient les variables CSS (couleurs, polices, espacements), les animations et les utilitaires partagés par tous les autres fichiers via `var()`.

---

## 5. Architecture CSS — Tableau de responsabilité

| Fichier CSS | Responsabilité | Éléments gérés |
|---|---|---|
| `base.css` | Fondation globale | `:root` variables, reset CSS, styles body, import Google Fonts, classes utilitaires, animations CSS, responsive global |
| `header.css` | Navigation principale | Header sticky, nav, logo, liens, CTA gradient, sélecteur de langue (FR/EN), hamburger mobile (checkbox hack) |
| `hero.css` | Section d'accroche | Titre animé (gradient shift), particules CSS, courbes décoratives SVG, stats social proof, boutons CTA, filtre bleu sur image |
| `about.css` | Présentation NexaLab | Layout 2 colonnes, texte de mission, image avec border glow, 3 cartes ADN (Modernité, Rigueur, Impact) avec icônes SVG |
| `services.css` | Expertises | Cards premium avec glow hover, icônes gradient, tags pill, accent line au survol |
| `stats.css` | Chiffres clés | Compteurs en gradient text, bande unifiée, divider animé au hover |
| `team.css` | Équipe / Partenaires | Avatars dynamiques avec hover lift, role tags, logos partenaires en grille |
| `team-membres.css` | Photos des membres | Photos circulaires, glassmorphisme, shine effect, badge rôle |
| `testimonials.css` | Témoignages | Cards citations, grand guillemet décoratif, barre accent au hover, étoiles |
| `contact.css` | Formulaire de contact | Inputs avec focus glow, textarea, labels uppercase, bouton gradient avec hover lift |
| `footer.css` | Pied de page | Brand gradient text, colonnes de liens avec underline hover, icônes sociales SVG, barre copyright |

---

## 6. Identité visuelle

La palette de NexaLab repose sur deux niveaux de lecture : des fonds profonds qui installent la crédibilité technologique, et des accents chromatiques qui guident l'action et signalent l'innovation.

### Palette de couleurs

| Nom | Variable CSS | Hex | Usage |
|---|---|---|---|
| **Background** | `--color-bg` | `#0b0f19` | Fond principal — profondeur, ancrage |
| **Background Alt** | `--color-bg-alt` | `#0d1120` | Surfaces secondaires (about, stats, testimonials) |
| **Card** | `--color-bg-card` | `#111827` | Fond des cartes et éléments interactifs |
| **Primary** | `--color-primary` | `#3b77df` | Accent principal — CTA, liens, bordures actives |
| **Accent** | `--color-accent` | `#60a5fa` | Accent secondaire — labels, highlights, gradient |
| **Text** | `--color-text` | `#f8fafc` | Titres, textes importants |
| **Text Muted** | `--color-text-muted` | `#94a3b8` | Corps de texte, descriptions |
| **Border** | `--color-border` | `#1e293b` | Bordures subtiles, séparateurs |

```css
/* Déclaration dans base.css */
:root {
  --color-primary:       #3b77df;
  --color-accent:        #60a5fa;
  --color-bg:            #0b0f19;
  --color-bg-alt:        #0d1120;
  --color-bg-card:       #111827;
  --color-text:          #f8fafc;
  --color-text-muted:    #94a3b8;
  --color-border:        #1e293b;
}
```

**Justification des choix :**
Le fond sombre (#0b0f19) installe immédiatement un registre technologique sérieux, cohérent avec l'audience cible (décideurs, investisseurs). Le bleu primary (#3b77df) guide l'œil vers les actions principales (CTA, chiffres clés) avec un contraste fort sur fond sombre. L'accent clair (#60a5fa) identifie visuellement tout ce qui touche à l'innovation et à la tech, créant un second niveau de lecture sans surcharger la hiérarchie.

---

## 7. Typographie

| Famille | Variable CSS | Usage | Caractéristique |
|---|---|---|---|
| **Syne** | `--font-display` | Titres (h1 à h3) | Géométrique, dense, autorité immédiate |
| **Inter** | `--font-body` | Corps de texte, descriptions | Légère, fluide, lecture confortable |

```css
/* Import dans base.css */
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=Syne:wght@600;700;800&display=swap');

:root {
  --font-display: 'Syne', sans-serif;
  --font-body:    'Inter', -apple-system, sans-serif;
}
```

**Justification :** Syne impose une présence forte sur les grands titres avec ses formes géométriques audacieuses ; Inter assure le confort de lecture sur de longs passages grâce à son dessin optimisé pour les écrans, essentiel pour les sections About, Services et Témoignages.

---

## 8. Décisions techniques

### Zéro JavaScript, zéro framework

Le cahier des charges impose HTML5 + CSS3 uniquement. Aucun JavaScript, aucun framework CSS (pas de Bootstrap, pas de Tailwind) n'est utilisé. Toutes les interactions sont réalisées en CSS pur.

### Iconographie — SVG inline

Les icônes sont intégrées directement en SVG inline dans le HTML. Ce choix élimine toute dépendance externe (pas de Font Awesome, pas de CDN), garantit un contrôle total sur les couleurs via `currentColor` et `stroke`, et respecte la contrainte « aucun framework ».

### Interactions CSS — Checkbox Hack

Les interactions sans JavaScript reposent sur le **checkbox hack** :
- **Menu hamburger mobile** : un `<input type="checkbox">` caché contrôle l'ouverture du menu latéral via le sélecteur `~`
- **Sélecteur de langue** : un second checkbox ouvre/ferme le dropdown FR/EN

### Traduction FR/EN — Deux fichiers HTML

Sans JavaScript, la traduction dynamique est impossible. Le site existe en deux versions :
- `index.html` — version française
- `index-en.html` — version anglaise

Le sélecteur de langue (globe SVG dans le header) contient des liens `<a>` qui redirigent simplement vers l'autre fichier.

### Animations — CSS pur

Toutes les animations sont réalisées avec `@keyframes` et les propriétés `animation` / `transition` CSS :
- Gradient shift sur le titre hero
- Particules flottantes (8 `<span>` animés individuellement)
- Shimmer sweep sur les badges et CTA
- Grille de fond en mouvement continu
- Halo lumineux pulsant
- Hover effects sur toutes les cartes (translateY, box-shadow, border-color)

### Courbes décoratives — SVG intégré

Deux courbes Bézier SVG encadrent le hero en forme d'entonnoir, partant des coins supérieurs et convergeant vers le centre. Elles utilisent `preserveAspectRatio="none"` pour s'adapter à toutes les tailles d'écran.

### Layout — Flexbox + CSS Grid

La mise en page combine **Flexbox** (navigation, hero, about, footer) et **CSS Grid** (services 3 colonnes, team 2 colonnes, membres 4 colonnes, stats responsive 2×2 → 1 colonne).

### Responsive — Breakpoints

Le design s'adapte à trois tailles d'écran avec des variables CSS qui changent selon le breakpoint :

```css
/* Breakpoints utilisés */
/* Mobile  : 480px et moins  → padding réduit, colonnes simples     */
/* Tablette: 768px et moins  → layouts en colonnes, gaps réduits     */
/* Desktop : plus de 1024px  → layout complet multi-colonnes         */
```

Les variables `--container-p`, `--space-3xl`, `--space-2xl`, etc. sont redéfinies dans les media queries de `base.css` pour un ajustement global cohérent.

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
6. **Penser à dupliquer les changements dans `index-en.html`** avec les traductions

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
