# NEXALAB — Document de Contexte Projet
> Ce document sert de contexte complet pour toute assistance IA sur le projet NexaLab.
> Il contient tout ce qu'une IA doit savoir pour générer du code, des textes ou des suggestions pertinentes et cohérentes avec le projet.

---

## 1. Présentation du projet

### Qu'est-ce que ce site ?

NexaLab est le site vitrine d'un **laboratoire d'innovation technologique africain**. C'est une page d'accueil unique (`index.html`) conçue pour représenter l'identité, les services et la crédibilité de NexaLab auprès de ses visiteurs cibles.

Le site est construit en **HTML5 et CSS3 uniquement** — sans JavaScript, sans framework, sans template extérieur. Chaque ligne de code est écrite à la main, dans le respect des standards du web moderne.

Il s'agit d'un projet étudiant réalisé dans le cadre du **Bloc 2 de l'Académie de Programmation de l'IFRI (Institut de Formation et de Recherche en Informatique)**, niveau L1. Le projet est compétitif : 6 groupes s'affrontent pour livrer la meilleure version du site. Une seule version sera retenue.

---

## 2. Le client — Qui est NexaLab ?

NexaLab est un **laboratoire fictif spécialisé dans l'innovation technologique pour les entreprises africaines**.

### Sa mission

NexaLab accompagne les entreprises africaines dans leur transformation numérique en leur proposant des solutions technologiques concrètes, modernes et adaptées à leur contexte. En d'autres termes : NexaLab identifie les problèmes opérationnels des entreprises et leur apporte des réponses technologiques — que ce soit via l'intelligence artificielle, l'analyse de données, l'IoT ou d'autres expertises tech.

### Son ADN

- **Modernité** — NexaLab est tourné vers l'avenir. Leurs solutions sont à la pointe.
- **Rigueur** — Chaque projet est traité avec sérieux, méthode et professionnalisme.
- **Impact** — L'objectif n'est pas la technologie pour la technologie, mais des résultats concrets pour les entreprises.

### Son positionnement

NexaLab se positionne comme un **partenaire de confiance** pour les décideurs africains qui veulent intégrer la technologie dans leur activité sans se perdre dans la complexité. Ce n'est pas un fournisseur de logiciels. C'est un laboratoire qui pense, conçoit et déploie des solutions sur mesure.

---

## 3. Pour qui construit-on ce site ?

Le site s'adresse à trois types de visiteurs distincts, et le design doit convaincre chacun d'eux **en moins de 10 secondes** :

### 👔 Les Directeurs d'entreprise
Ce sont les clients principaux de NexaLab. Ils ont des problèmes concrets à résoudre dans leur entreprise et cherchent un partenaire tech fiable. Ils veulent voir : la crédibilité, les services proposés, des preuves de résultats (chiffres, témoignages).

### 💰 Les Investisseurs
Ils évaluent le potentiel de NexaLab. Ils cherchent une structure solide, une vision claire, une équipe compétente. Ils veulent voir : le sérieux, la vision, la structure organisationnelle.

### 👨‍💻 Les Jeunes talents tech
Ils envisagent de rejoindre NexaLab. Ils veulent savoir si c'est un endroit stimulant et ambitieux. Ils cherchent : la culture d'entreprise, les projets, l'équipe.

---

## 4. Pourquoi construit-on ce site ?

### Objectif principal
Donner à NexaLab une **présence web professionnelle et crédible** qui reflète son niveau d'ambition. Le site est leur vitrine digitale — c'est la première impression qu'auront les décideurs, les investisseurs et les talents.

### Ce que le site doit accomplir
1. **Convaincre** — Un visiteur qui arrive doit immédiatement comprendre qui est NexaLab et pourquoi lui faire confiance.
2. **Informer** — Présenter clairement les services, l'équipe, les chiffres clés.
3. **Engager** — Pousser le visiteur à passer à l'action : remplir le formulaire de contact, envoyer un message.

### Ce que le site ne doit PAS faire
- Être générique ou ressembler à un template quelconque.
- Être surchargé visuellement.
- Être lent, cassé sur mobile ou difficile à lire.

---

## 5. Sections obligatoires du site

Le site contient exactement **9 sections** dans `index.html` :

| # | Section | Contenu attendu |
|---|---|---|
| 1 | **Header & Navigation** | Logo NexaLab + menu de navigation |
| 2 | **Hero Section** | Message d'accroche fort + sous-titre + call-to-action |
| 3 | **À propos / Mission** | Qui est NexaLab, leur vision, ce qui les différencie |
| 4 | **Services / Expertises** | Minimum 3 services avec icônes (IA, IoT, Data...) |
| 5 | **Chiffres clés** | Statistiques marquantes (projets, partenaires, pays...) |
| 6 | **Équipe ou Partenaires** | Présentation de l'équipe core OU logos partenaires |
| 7 | **Témoignages** | 3 retours clients crédibles et bien mis en page |
| 8 | **Formulaire de contact** | Nom, email, sujet, message — inputs stylisés |
| 9 | **Footer** | Liens, réseaux sociaux, copyright, email |

---

## 6. Identité visuelle — Palette de couleurs

### 🎨 Palette officielle du projet

| Rôle | Nom | Code HEX | Utilisation |
|---|---|---|---|
| Couleur d'action | Bleu principal | `#3b77df` | Boutons CTA, liens actifs, accents, hover |
| Fond principal | Bleu sombre | `#1d2733` | Arrière-plan général du site |
| Fond header | Noir doux | `#0f1117` | Fond du header et de la navigation |

### Couleurs complémentaires recommandées

Ces couleurs ne sont pas imposées mais fortement recommandées pour compléter la palette :

| Rôle | Code HEX | Utilisation |
|---|---|---|
| Texte principal | `#ffffff` | Titres, textes sur fond sombre |
| Texte secondaire | `#a0aec0` | Sous-titres, descriptions, textes discrets |
| Fond de carte | `#243447` | Cards, sections légèrement surélevées |
| Bordure subtile | `#2d3f53` | Séparateurs, bordures de cards |

### Variables CSS à utiliser dans `base.css`

```css
:root {
  /* Couleurs principales */
  --color-primary: #3b77df;
  --color-bg: #1d2733;
  --color-bg-header: #0f1117;
  --color-bg-card: #243447;

  /* Textes */
  --color-text: #ffffff;
  --color-text-muted: #a0aec0;

  /* Bordures */
  --color-border: #2d3f53;

  /* États */
  --color-primary-hover: #2d62c4;
}
```

### Logique d'application des couleurs

- Le **fond général** du site est `#1d2733` — bleu sombre, professionnel, tech.
- Le **header** a son propre fond `#0f1117` — plus sombre pour créer une séparation visuelle nette avec le reste du site.
- Les **boutons d'action** (CTA) utilisent `#3b77df` — le bleu vif qui attire l'œil sur les éléments cliquables.
- Le **texte** est blanc `#ffffff` pour les titres et gris clair `#a0aec0` pour les textes secondaires.

---

## 7. Ton et style rédactionnel

Quand tu génères du contenu textuel pour ce site, respecte ces règles :

- **Confiant** — NexaLab ne doute pas. Pas de "nous essayons de", mais "nous livrons".
- **Innovant** — Le vocabulaire est moderne et technologique sans être incompréhensible.
- **Accessible** — Les décideurs africains ne sont pas tous des ingénieurs. Parle clairement.
- **Direct** — Pas de phrases creuses. Chaque phrase doit dire quelque chose.

### Exemples de ton

| ❌ À éviter | ✅ À utiliser |
|---|---|
| "Nous essayons de proposer des solutions..." | "Nous livrons des solutions qui fonctionnent." |
| "Notre équipe est passionnée par la tech..." | "Nous transformons la technologie en avantage compétitif." |
| "Contactez-nous pour en savoir plus." | "Parlons de votre projet. Maintenant." |

---

## 8. Contraintes techniques importantes

Toute suggestion de code doit respecter ces règles absolues :

- ✅ **HTML5 sémantique uniquement** — utiliser `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`. Jamais une `<div>` là où une balise sémantique convient.
- ✅ **CSS modulaire** — chaque section a son propre fichier CSS. Ne jamais tout mettre dans un seul fichier.
- ✅ **Flexbox obligatoire** pour la mise en page principale. Grid autorisé en complément.
- ✅ **Responsive design** — breakpoints à 768px (mobile) et 1024px (tablette).
- ✅ **Classes en anglais** — nommage logique et descriptif (ex: `.hero__title`, `.nav__link`).
- ❌ **Aucun JavaScript** — même pour les animations ou les menus hamburger.
- ❌ **Aucun framework CSS** — pas de Bootstrap, Tailwind ou autre.
- ❌ **Aucun template copié** — tout le code est original.

---

## 9. Sections dont je suis responsable

Dans le cadre de la répartition du travail au sein du groupe, je suis responsable des sections suivantes :

| Section | Fichier CSS associé |
|---|---|
| Header & Navigation | `styles/header.css` |
| Hero Section | `styles/hero.css` |
| À propos / Mission | `styles/about.css` |

### Ce que l'IA doit savoir sur ces sections

**Header & Navigation**
- Contient le logo NexaLab et le menu de navigation.
- Fond : `#0f1117` (noir doux) — plus sombre que le reste du site.
- Le header peut être sticky (fixé en haut lors du scroll).
- Le menu contient les liens vers les différentes sections de la page.

**Hero Section**
- C'est la première chose que voit le visiteur — elle est critique.
- Elle doit contenir : un titre d'accroche fort, un sous-titre, et un bouton CTA.
- Le bouton CTA est en `#3b77df`.
- Le fond suit le fond général du site : `#1d2733`.

**À propos / Mission**
- Présente qui est NexaLab, leur vision et ce qui les différencie.
- Ton sérieux et inspirant.
- Peut contenir une image ou un visuel illustratif.

---

*Document rédigé comme contexte IA pour le projet NexaLab — Académie de Programmation IFRI, Bloc 2.*
