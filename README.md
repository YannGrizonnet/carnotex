# CarnoTeX

> A modular LaTeX toolkit for mathematics teaching.

CarnoTeX est une collection de packages LaTeX destinée à la rédaction de documents pédagogiques de mathématiques.

Développé à l'origine pour un usage personnel, il fournit un ensemble cohérent de commandes pour produire des cours, TD, exercices, évaluations, présentations Beamer et documents destinés à l'impression ou à la projection.

---

# Principales fonctionnalités

- Architecture modulaire
- Théorèmes et environnements mathématiques
- Outils pédagogiques (objectifs, prérequis, notes...)
- Gestion de plusieurs versions d'un même document (élève, professeur, notes)
- Charte graphique homogène
- Compatibilité avec les anciens documents grâce au package `carnolegacy`

---

# Architecture

Le projet est composé de plusieurs packages.

| Package | Rôle |
|----------|------|
| `carnotex` | noyau du package |
| `carnomath` | commandes et environnements mathématiques |
| `carnopeda` | outils pédagogiques |
| `carnolegacy` | compatibilité avec les anciens documents |

---

# Installation

Copiez le dossier `tex/` dans votre arbre TEXMF personnel.

Par exemple sous Linux :

```text
~/texmf/tex/latex/CarnoTeX
```

ou créez un lien symbolique vers le dépôt Git :

```bash
ln -s ~/Git/CarnoTeX/tex ~/texmf/tex/latex/CarnoTeX
```

---

# Premier document

```latex
\documentclass{article}

\usepackage[all]{carnotex}
\level{eleve}

\begin{document}

\df*{
Toute fonction affine est continue.
}

\end{document}
```

---

# Documentation

La documentation complète est disponible dans :

```
doc/Guide-CarnoTeX.pdf
```

Elle décrit l'ensemble des commandes publiques du projet.

---

# Exemples

Le dossier `examples/` contient plusieurs documents complets illustrant l'utilisation de CarnoTeX :

- cours
- TD
- DS
- QCM AMC
- Beamer

---

# Tests

Le dossier `tests/` contient les documents de validation des différents packages.

Ils permettent de vérifier que toutes les commandes compilent correctement après une modification.

---

# Compatibilité

CarnoTeX est principalement développé avec **LuaLaTeX**.

Le package `carnolegacy` permet de compiler d'anciens documents utilisant notamment PSTricks ou des commandes historiques.

---

# Licence

À définir.

---

# Auteur

Yann Grizonnet