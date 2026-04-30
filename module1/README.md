 🔍 Le Code que tu n'as pas écrit
### Analyse du code source — DevStart Agency

> Module 1 · Bloc 2 — Génie Logiciel  
> Académie de Programmation · IFRI · L1 Intelligence Artificielle · 2025–2026

---

## 👥 Groupe n°8

| Nom | Prénom |
|-----|--------|
| SOZAN | Euloge |
| JORDY | Mayel |
| DJEHONNON | Géoffroy |
| TONATO | Océane |

---

## 📌 Contexte du projet

La startup fictive **DevStart Agency** nous a transmis le code source d'une mini-application web développée par un stagiaire qui vient de partir. Le livrable se compose de deux fichiers : `index.html` et `style.css`. Il s'agit d'une page vitrine présentant les services de l'agence, une section à propos, des témoignages clients et un formulaire de contact.

Notre mission : **analyser, comprendre et documenter** ce code avant que l'équipe puisse le reprendre.

---

## 🗂️ Structure du dépôt

```
📦 devstart-analyse/
├── 📁 original/          # Code source tel que reçu, sans aucune modification
│   ├── index.html
│   └── style.css
│
├── 📁 annotated/         # Code source avec nos commentaires et annotations
│   ├── index.html
│   └── style.css
│
├── 📄 rapport.pdf        # Rapport d'analyse final (Groupe 8)
└── 📄 README.md          # Ce fichier
```

---

## 🔎 Notre démarche

### Phase 1 — Exploration (Jours 1–2)
Lecture complète du code sans rien modifier. Nous avons annoté chaque section dans nos propres mots et listé le rôle supposé de chaque classe et bloc HTML.

### Phase 2 — Analyse critique (Jours 3–4)
Identification des problèmes de lisibilité, d'organisation et de fonctionnalité. Chaque problème a été argumenté et classé par niveau de priorité.

### Phase 3 — Rapport & Présentation (Jour 5)
Rédaction du rapport structuré et préparation de la présentation orale de 10 minutes.

---

## ⚠️ Principaux problèmes identifiés

| # | Problème | Impact | Priorité |
|---|----------|--------|----------|
| 1 | Nommage cryptique des classes CSS (`b1`, `c1a`, `d0`…) | Maintenabilité nulle | 🔴 HAUTE |
| 2 | Classes individuelles au lieu de classes partagées | Évolution risquée | 🔴 HAUTE |
| 3 | Absence de balises sémantiques HTML5 | SEO et accessibilité | 🟡 MOYENNE |
| 4 | Formulaire de contact non fonctionnel (pas de `<form>`) | Fonctionnalité cassée | 🔴 HAUTE |
| 5 | Images sans attribut `alt` + fichiers manquants | Accessibilité + visuel cassé | 🟡 MOYENNE |
| 6 | Couleurs codées en dur sans variables CSS | Évolutivité compromise | 🟢 FAIBLE |
| 7 | Aucune media query — site inutilisable sur mobile | Site cassé sur mobile | 🔴 HAUTE |
| 8 | CSS sans commentaires explicatifs | Compréhension difficile | 🟢 FAIBLE |

> Le détail complet de chaque problème, avec exemples de code et propositions d'amélioration, est disponible dans le **rapport PDF**.

---

## 📄 Rapport d'analyse

Le rapport complet est disponible à la racine du dépôt : [`rapport.pdf`](./rapport.pdf)

Il couvre :
- Description globale du code (structure, technologies, palette graphique)
- Analyse critique approfondie — problème par problème
- Tableau de synthèse avec niveaux de priorité
- Recommandations concrètes pour l'équipe DevStart

---

## 💡 Recommandations principales

1. **Corriger le formulaire de contact** — ajouter `<form>`, corriger `type="email"`, marquer les champs obligatoires (`required`). C'est la seule fonctionnalité cassée.
2. **Ajouter les media queries** pour le responsive. Sur mobile, le site est actuellement illisible.
3. **Renommer toutes les classes CSS** selon la convention BEM avant d'ajouter la moindre ligne de code.
4. **Introduire des variables CSS** (`:root`) pour les couleurs et factoriser les styles groupés en classes réutilisables.
5. **Ajouter les balises sémantiques HTML5**, les attributs `alt` sur les images et intégrer les fichiers images manquants.

---

## 🛠️ Technologies analysées

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)

---

## 📅 Informations

- **Date de rendu** : Vendredi 17 avril 2026  
- **Établissement** : Institut de Formation et de Recherche en Informatique (IFRI) — Abomey-Calavi  
- **Module** : Bloc 2 · Module 1 — Génie Logiciel  
- **Encadrement** : Académie de Programmation IFRI
