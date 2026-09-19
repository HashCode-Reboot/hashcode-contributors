# GitHub Projects — Modèle de pilotage HashCode

## Objectif

GitHub Projects sert à suivre l'avancement du portefeuille Global Impact sans transformer chaque dépôt en système isolé.

Le principe retenu est :

```text
HashCode Contributors
        ↓
Missions / Contributions
        ↓
GitHub Issues & Pull Requests
        ↓
GitHub Projects
        ↓
Projets Global Impact
        ↓
Pilotes / Mesures d'impact
```

## Architecture recommandée

### 1. HashCode Global Impact

Projet principal de portefeuille. Il rassemble les Issues et Pull Requests des 15 dépôts.

Vues recommandées :

- **Portfolio** — vue d'ensemble des 15 projets
- **Kanban Global** — suivi par phase
- **Web & Software** — filtre domaine Web
- **Cybersecurity** — filtre domaine Cyber
- **Applied AI** — filtre domaine AI
- **Risks & Blockers** — éléments bloqués ou à risque
- **Impact** — éléments liés à une mesure ou une preuve d'impact

### 2. HashCode Contributors

Projet consacré aux missions, candidatures, contributions et progression des contributors.

Il doit rester distinct du portefeuille produit, tout en permettant de relier une mission à un dépôt et à une Issue.

### 3. Vues par projet

Il n'est pas nécessaire de créer 15 Projects indépendants. Une vue filtrée par dépôt dans le projet Global Impact fournit un Kanban propre à chaque projet tout en conservant la vision portefeuille.

Exemples :

- CivicOS
- HealthGrid
- FoodFlow
- SkillGraph
- Resilience
- CyberShield
- ScamShield
- CyberThreat Atlas
- Incident Response
- Digital Safety
- African Language AI
- AI Tutor
- AgroAI
- MedAI
- Knowledge Engine

## Workflow standard

```text
BACKLOG
   ↓
RESEARCH
   ↓
VALIDATION
   ↓
READY
   ↓
IN DEVELOPMENT
   ↓
REVIEW
   ↓
PILOT
   ↓
MEASURE
   ↓
DONE
```

### Définitions

| Statut | Signification |
|---|---|
| BACKLOG | Idée ou travail identifié mais non engagé |
| RESEARCH | Recherche, exploration ou collecte d'informations |
| VALIDATION | Vérification du problème, des hypothèses ou des besoins |
| READY | Travail suffisamment défini pour être exécuté |
| IN DEVELOPMENT | Construction en cours |
| REVIEW | Revue technique, produit, sécurité ou contenu |
| PILOT | Test avec des utilisateurs ou un contexte réel |
| MEASURE | Collecte et analyse des résultats |
| DONE | Livrable terminé et critères d'acceptation satisfaits |

## Champs recommandés

Chaque item du Project devrait pouvoir être caractérisé par :

- **Status** — phase actuelle
- **Project** — projet concerné
- **Domain** — Web, Cybersecurity, Applied AI
- **Priority** — priorité opérationnelle
- **Phase** — Discovery, Validation, Build, Pilot, Impact
- **Contributor Level** — Candidat, Contributor, Contributor actif, Core Contributor, Lead
- **Impact Area** — domaine de problème traité
- **Effort** — estimation relative
- **Owner** — responsable de l'item
- **Milestone** — jalon associé
- **Impact KPI** — indicateur suivi
- **Evidence** — lien vers une preuve ou un résultat
- **Risk** — niveau de risque ou blocage

## Règles de gestion

1. Une idée n'est pas automatiquement un projet.
2. Un projet n'avance vers `READY` qu'après clarification du problème et du livrable.
3. Une Issue doit avoir un objectif et des critères d'acceptation compréhensibles.
4. Une Pull Request doit être reliée à une Issue lorsqu'elle implémente un travail suivi.
5. Les décisions importantes doivent être documentées dans le dépôt concerné.
6. Un projet ne passe pas à `DONE` uniquement parce que le code compile : le livrable et ses critères d'acceptation doivent être vérifiés.
7. Pour les projets à impact, `PILOT` et `MEASURE` sont des étapes à part entière.
8. Les preuves d'impact doivent être conservées et référencées lorsqu'elles existent.

## Relation avec HashCode Contributors

Le système de contribution suit cette chaîne :

```text
Candidat
  ↓
Mission
  ↓
Issue
  ↓
Contribution
  ↓
Pull Request
  ↓
Review
  ↓
Merge
  ↓
Progression Contributor
```

Pour un projet à impact :

```text
Problème
  ↓
Recherche
  ↓
Hypothèse
  ↓
Validation
  ↓
Prototype
  ↓
Pilote
  ↓
Mesure
  ↓
Preuve
  ↓
Itération / Scale
```

## Mise en place dans GitHub

Les Projects d'organisation sont des ressources GitHub distinctes des fichiers d'un dépôt. Le connecteur GitHub actuellement disponible pour HashCode permet de gérer les dépôts, fichiers, Issues et Pull Requests, mais n'expose pas d'opération d'écriture pour créer/configurer un GitHub Project.

La configuration du Project doit donc être effectuée dans l'interface GitHub de l'organisation, en utilisant exactement le modèle défini dans ce document.

### Configuration minimale

1. Créer `HashCode Global Impact` au niveau de l'organisation.
2. Ajouter les Issues et Pull Requests des 15 dépôts.
3. Créer les statuts du workflow standard.
4. Ajouter les champs `Project`, `Domain`, `Priority`, `Phase`, `Owner`, `Impact KPI` et `Risk`.
5. Créer les vues Portfolio, Kanban Global et les vues filtrées par domaine.
6. Créer une vue filtrée pour chacun des 15 dépôts.
7. Créer séparément `HashCode Contributors` pour les missions et contributions.
8. Relier les missions de `hashcode-contributors` aux Issues des dépôts opérationnels.

## Convention de nommage

Projects :

- `HashCode Global Impact`
- `HashCode Contributors`

Vues :

- `Portfolio`
- `Kanban Global`
- `Web & Software`
- `Cybersecurity`
- `Applied AI`
- `Risks & Blockers`
- `Impact`
- `Project — <nom>`

## Résultat attendu

Le pilotage doit permettre de répondre rapidement à cinq questions :

1. Quels projets existent ?
2. Où en est chaque projet ?
3. Qui contribue et sur quelle mission ?
4. Qu'est-ce qui bloque ?
5. Quelle preuve montre que le travail produit un résultat ?

Le Project n'est pas la source de vérité du produit : **les dépôts restent les sources de vérité du code et de la documentation**. Le Project est la couche de pilotage transversal.