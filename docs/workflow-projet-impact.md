# Workflow — Projets à impact

```mermaid
stateDiagram-v2
 [*] --> Problem
 Problem --> Research
 Research --> Validation
 Validation --> Prototype
 Prototype --> Pilot
 Pilot --> Measurement
 Measurement --> Iterate
 Iterate --> Pilot
 Measurement --> Scale
 Measurement --> Stop
 Scale --> [*]
 Stop --> [*]
```

## Règles

### Problem
Le problème doit être formulé avec des personnes concernées et des éléments vérifiables.

### Research
Identifier ce qui existe déjà, les contraintes, les acteurs, les alternatives et les risques de duplication.

### Validation
Obtenir des retours terrain avant d'investir fortement dans l'implémentation.

### Prototype
Construire uniquement ce qui permet de tester l'hypothèse.

### Pilot
Tester dans un contexte réel contrôlé avec des critères préétablis.

### Measurement
Comparer les résultats à une situation de référence. Documenter résultats positifs, négatifs et inattendus.

### Iterate / Scale / Stop
Un projet peut être amélioré, déployé plus largement ou arrêté. L'arrêt d'un prototype qui ne valide pas l'hypothèse est un résultat utile s'il est correctement documenté.

## Relation avec Contributors

Le dépôt `hashcode-contributors` fournit les missions, le parcours, la gouvernance et les règles de contribution. Les dépôts projet portent le code, les données, les expériences et la documentation spécifique.
