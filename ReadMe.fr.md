<img width="1280" height="640" alt="logo3" src="https://repository-images.githubusercontent.com/1299189033/ba2bd2de-4547-458c-9898-bd63c488ea35" />

# Brainstorming-Plus V2

> Un partenaire de réflexion cognitive de haut niveau pour l'idéation, la pensée stratégique, la résolution de problèmes et l'évaluation d'idées.

[![skills.sh](https://img.shields.io/badge/skills.sh-Registry-000000?logo=vercel&logoColor=white)](https://www.skills.sh/bibo3002/brainstorming-plus/brainstorming-plus)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Version](https://img.shields.io/badge/version-2.0.0-blue)]()

[English](ReadMe.md) | **Français** | [العربية](ReadMe.ar.md)

---

## 🤖 Qu'est-ce que Brainstorming-Plus ?

Brainstorming-Plus est un partenaire de réflexion de haut niveau — agissant tour à tour comme **facilitateur de conception**, **réviseur senior** ou **partenaire de sparring critique**. Contrairement à un simple outil d'exécution, ce Skill a pour but de vous pousser dans vos retranchements, d'apporter des angles inattendus et de vous aider à aboutir à des idées que vous n'auriez pas atteintes seul.

Il transforme votre assistant IA (Codex, OpenCode, Claude, etc.) en un partenaire stratégique senior qui empêche la convergence prématurée, remet en question les prémisses erronées et vous guide à travers des phases cognitives structurées.

### 🧠 Logique & Philosophie

La logique fondamentale de ce Skill repose sur une **interaction structurée** et une **opinion affirmée** :

| Principe | Description |
|----------|-------------|
| **Partenaire, pas bâtisseur** | Le Skill ne code pas et ne modifie pas les comportements durant la phase de réflexion ; il se concentre exclusivement sur la conception et la validation intellectuelle. |
| **Contradiction constructive** | Conçu pour remettre en question vos hypothèses (« Cela suppose X — en sommes-nous sûrs ? ») et éviter la convergence précoce vers une solution. |
| **Divergence avant convergence** | Encourage l'exploration de multiples options avant de s'arrêter sur un choix définitif. |

### 🎯 Finalités

- Transformer des idées brutes en **spécifications validées** par un dialogue structuré.
- Éviter les pièges courants (anti-patterns) tels que le développement de solutions avant d'avoir défini le problème, ou le piège de la parité fonctionnelle avec la concurrence.
- Garantir la clarté partagée sur le **« quoi »**, le **« pourquoi »** et le **« pour qui »** avant d'écrire la moindre ligne de code.
- Assurer une **rigueur technique** en intégrant systématiquement des exigences non fonctionnelles (performance, échelle, sécurité).

---

## 🎯 Quand l'utiliser

✅ Réfléchir à un problème ou générer/affiner des idées
✅ Remettre en question une hypothèse ou peser des compromis
✅ Planifier un projet, une fonctionnalité ou une initiative stratégique
✅ Traverser une décision ambiguë ou ouverte
✅ Obtenir un second avis ou sortir d'une boucle mentale
✅ Structurer une décision (options → risques → compromis → prochaines étapes)

### Modes de Brainstorming Adaptatifs

Le Skill adapte son comportement selon l'état de votre réflexion :

| Mode | Quand |
|------|-------|
| **Exploration de Problème** | Le problème n'est pas encore défini |
| **Idéation de Solution** | Le problème est clair mais nécessite des idées divergentes |
| **Test d'Hypothèses** | Stress-tester une direction déjà choisie |
| **Exploration Stratégique** | Décisions à long terme et positionnement |

## 🚫 Quand NE PAS l'utiliser

❌ Recherches factuelles simples
❌ Génération de code directe avec un cahier des charges clair
❌ Tâches nécessitant uniquement l'exécution d'un plan déjà validé

---

## 📦 Installation Globale (Multi-Agents)

Les Agent Skills étant standardisés autour du format `SKILL.md`, vous pouvez installer Brainstorming-Plus globalement pour qu'il soit disponible dans **tous** vos projets.

### Option 1 : Registre `skills.sh` (Recommandé)

```bash
npx skills add bibo3002/brainstorming-plus --global
```

### Option 2 : Installation Manuelle

Clonez ce dépôt et copiez-le dans le répertoire global de votre agent :

| Agent / Plateforme | Répertoire Global |
| :--- | :--- |
| **OpenAI Codex CLI** | `~/.agents/skills/brainstorming-plus/` |
| **OpenCode** | `~/.config/opencode/skills/brainstorming-plus/` |
| **Claude Code** | `~/.claude/skills/brainstorming-plus/` |

```bash
# Commande bash universelle pour l'installation globale
git clone https://github.com/bibo3002/brainstorming-plus.git /tmp/brainstorming-plus

# Pour Codex CLI
cp -r /tmp/brainstorming-plus ~/.agents/skills/

# Pour OpenCode
cp -r /tmp/brainstorming-plus ~/.config/opencode/skills/

# Pour Claude Code
cp -r /tmp/brainstorming-plus ~/.claude/skills/
```

---

## 🏗️ Architecture de Base

Brainstorming-Plus V2 est gouverné par **deux couches indépendantes et interactives** :

| Couche | Rôle | Question |
|--------|------|----------|
| **Couche de Gouvernance** | Structure du processus : cadrage, clarification socratique, Understanding Lock, alternatives, compromis, journal de décision, handoff | *Où en sommes-nous ?* |
| **Moteur Cognitif** | Intelligence adaptative : sélectionne la prochaine intervention cognitive via routage heuristique, escalade progressive et détection de convergence | *Quel type de réflexion est nécessaire maintenant ?* |

### Les Trois Axes de Contrôle

| Axe | Question | Valeurs |
|-----|----------|---------|
| **État du Processus** | Où en sommes-nous ? | Frame → Explore → Ideate → Evaluate → Decide → Handoff |
| **Lentille Cognitive** | Comment penser ? | Expand → Challenge → Transform → Reframe → Connect → Stress-test → Execute |
| **Mode de Contrôle** | Qui choisit ? | AUTO → GUIDED → MANUAL |

### États du Processus (Machine à États Gouvernée)

Le processus est une **machine à états gouvernée avec boucles contrôlées**, pas une séquence linéaire rigide :

```
Frame → Explore → Ideate → Evaluate → Decide
                                         │
                                         │ approbation utilisateur
                                         ▼
                                      Handoff
                                         │
                                         │ autorisation d'implémentation
                                         ▼
                                   Implémentation
```

### Les Sept Lentilles Cognitives

| Lentille | Question Centrale | Exemples de Techniques |
|----------|-------------------|----------------------|
| 🔍 **Expand** | « Quoi d'autre ? » | Starbursting, Brainwriting, Analogie |
| ⚔️ **Challenge** | « Notre réflexion est-elle fausse ? » | Avocat du Diable, Test d'Hypothèses |
| 🔧 **Transform** | « Comment muter ceci ? » | SCAMPER, Soustraction, Exagération |
| 🔄 **Reframe** | « Et si le problème était différent ? » | Cinq Pourquoi, Jobs-to-be-Done |
| 🔗 **Connect** | « Que se passe-t-il quand ils collisionnent ? » | Matrice Morphologique, Fusion |
| 🧪 **Stress-test** | « Survit-il à la réalité ? » | Pre-mortem, Cas Limites |
| 🚀 **Execute** | « Comment opérationnaliser ? » | Décomposition, Chemin Critique, MVP |

> 📖 Référence complète : [references/REFERENCE.md](references/REFERENCE.md)

### Outils & Frameworks Mobilisables

Selon les besoins, le Skill utilise des outils de pensée structurés comme :

- **Jobs-to-be-Done (JTBD)** — Comprendre les motivations profondes des utilisateurs.
- **SCAMPER** — Transformer un produit ou une idée existante.
- **Boucle OODA** — Prise de décision rapide en environnement compétitif.
- **Inversion (Reverse Brainstorming)** — Identifier les risques en imaginant comment faire échouer le projet.
- **Pre-mortem** — Supposer l'échec total et tracer les causes.
- **Cinq Pourquoi** — Tracer la cause racine d'un problème.

---

## ⚙️ Modes de Contrôle

| Mode | Comportement |
|------|-------------|
| **AUTO** (défaut) | L'IA sélectionne la lentille cognitive selon les signaux de diagnostic |
| **GUIDED** | L'IA recommande 2–3 lentilles ; vous choisissez |
| **MANUAL** | Vous sélectionnez explicitement la technique ; l'IA l'applique |

---

## 📊 Échelle de Complexité

| Niveau | Type | Sortie |
|--------|------|--------|
| **A — Micro** | Décisions rapides, réversibles | Problème → Options → Recommandation |
| **B — Standard** | Complexité modérée | Cadrage → Hypothèses → 2–3 approches → Compromis |
| **C — Complexe** | Multiples parties prenantes | Understanding Lock → NFRs → Approches → Decision Log |
| **D — Transformationnel** | Impact organisationnel, irréversible | Design Doc complet → Analyse de scénarios → Roadmap |

---

## 🔑 Règle d'Or : Séparation Lentille–Phase

> **La lentille Execute structure comment opérationnaliser une direction acceptée. Elle n'autorise PAS l'implémentation.**

| Concept | Signification | Peut produire du code ? |
|---------|--------------|------------------------|
| **Lentille Execute** | Penser comment transformer une direction en action | ❌ Non |
| **Handoff** | Empaqueter le raisonnement approuvé pour l'implémentation | 📦 Artefacts prêts |
| **Implémentation** | Transition du raisonnement vers la construction | ✅ Oui, si explicitement autorisé |

---

## 🚦 Critères de Sortie

Le Skill ne considère la session terminée que lorsque :

- ✅ Le design ou la décision est suffisamment développé et approuvé.
- ✅ Les risques sont reconnus.
- ✅ Le **Decision Log** est créé si applicable.
- ✅ Les incertitudes non résolues sont explicitement identifiées.
- ✅ L'utilisateur dispose de prochaines actions claires ou d'un Handoff défini.

---

## 📂 Structure des Fichiers

| Fichier | Rôle |
| :--- | :--- |
| `SKILL.md` | Définition principale du skill — gouvernance, lentilles, règles socratiques |
| `references/REFERENCE.md` | Arsenal Cognitif complet : 7 lentilles, Échelle d'Escalade, Table de Routage |
| `references/EXAMPLES.md` | 7 scénarios démontrant le comportement attendu |

---

## 📖 Exemples

Sept exemples détaillés démontrant le skill en action :

| # | Scénario | Comportement Validé |
|---|----------|-------------------|
| 01 | Décision simple (fournisseur) | Échelle de complexité + discipline de preuve |
| 02 | Prémisse erronée | Suffisance de prémisse + règle d'une question |
| 03 | Brainstorming stagnant | Détection de convergence + escalade conditionnelle |
| 04 | Architecture logicielle complexe | Understanding Lock + NFRs + machine à états |
| 05 | Transformation stratégique | Gouvernance complète + boucles + échelle |
| 06 | Sélection manuelle de technique | Override utilisateur + séparation lentille/technique |
| 07 | Preuve requise (question fiscale) | Suffisance de preuve + sortie recherche |

> 📖 Exemples complets : [references/EXAMPLES.md](references/EXAMPLES.md)

---

## 🤝 Contribution

Les contributions sont bienvenues ! Veuillez lire [CONTRIBUTING.md](CONTRIBUTING.md) au préalable.

## 📝 Changelog

Voir [CHANGELOG.md](CHANGELOG.md) pour l'historique des versions.

## 📄 Licence

Ce projet est sous licence [MIT](LICENSE).

## 👤 Auteur

**Habib Farhat** — Avocat Tunisien & Concepteur de Skills IA