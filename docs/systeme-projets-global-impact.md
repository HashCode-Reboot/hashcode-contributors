# HashCode Global Impact — Système de pilotage

## 1. Architecture

Les 15 projets sont regroupés en trois domaines : Web & Software, Cybersecurity et Applied AI. Chaque dépôt possède ses Issues et son historique, tandis que `hashcode-contributors` fournit le système commun de contribution.

```text
Global Portfolio
├── Web & Software (5)
├── Cybersecurity (5)
└── Applied AI (5)
       ↓
Project Repository
       ↓
Issues / PRs / Reviews
       ↓
Contributors
       ↓
Pilot
       ↓
Impact Evidence
```

## 2. Cycle standard

`BACKLOG → RESEARCH → VALIDATION → READY → IN DEVELOPMENT → REVIEW → PILOT → MEASURE → DONE`

Une issue ne passe à `READY` que lorsque son objectif, son contexte, son livrable et ses critères d'acceptation sont suffisamment précis.

## 3. Phases produit

### Foundation
Comprendre le problème avant de construire.

### Architecture
Définir domaines, données, interfaces, sécurité et contraintes.

### MVP
Construire un parcours de bout en bout, volontairement limité.

### Validation
Tester qualité, sécurité, utilisabilité et hypothèses métier.

### Pilot
Tester avec un petit groupe/territoire réel lorsque les conditions sont réunies.

### Measure
Comparer les résultats aux baselines et documenter les preuves.

### Scale
Étendre uniquement après apprentissage suffisant.

## 4. Structure recommandée des issues

Chaque issue doit préciser :
- Casquettes mobilisées
- Contexte
- Objectif
- Travail attendu
- Livrables
- Critères d'acceptation
- Dépendances
- Risques
- Preuve attendue

## 5. Release V0.1

Une V0.1 n'est pas une version complète. Elle doit démontrer un cas d'usage central de bout en bout, être documentée, testable et suffisamment contrôlée pour son contexte.

Checklist minimale :
- [ ] parcours principal fonctionnel
- [ ] données de démonstration ou dataset documenté
- [ ] tests critiques
- [ ] gestion des erreurs
- [ ] documentation d'installation
- [ ] sécurité de base
- [ ] limites connues
- [ ] changelog
- [ ] métriques de validation
- [ ] décision explicite sur le pilote

## 6. Mesure d'impact

Chaque projet doit définir au moins :
- une baseline
- un KPI de résultat
- une méthode de collecte
- une période de mesure
- une source de preuve

Le nombre de commits, étoiles ou lignes de code n'est pas un KPI d'impact.

## 7. Contribution

Toute contribution significative doit être traçable par une Issue et une PR lorsqu'elle modifie le code ou la documentation structurante.

`Issue → Branch → PR → Review → Merge → Release → Evidence`

## 8. Gouvernance

Les décisions structurantes doivent être documentées par ADR lorsque nécessaire. Les décisions métier sensibles doivent être validées par la casquette Domain Expert correspondante. Les sujets sécurité, confidentialité, santé et IA à risque nécessitent les reviews spécialisées appropriées.
