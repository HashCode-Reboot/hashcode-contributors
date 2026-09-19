# Cartographie des projets HashCode

Cette carte relie les projets d'impact, les domaines HashCode et le programme Contributor.

```mermaid
flowchart TB
 C[HashCode Contributors] --> G[Global Impact]
 G --> W[Web]
 G --> CY[Cyber]
 G --> AI[Applied AI]
 W --> W1[CivicOS]
 W --> W2[HealthGrid]
 W --> W3[FoodFlow]
 W --> W4[SkillGraph]
 W --> W5[Resilience]
 CY --> C1[CyberShield]
 CY --> C2[ScamShield]
 CY --> C3[CyberThreat Atlas]
 CY --> C4[Incident Response]
 CY --> C5[Digital Safety]
 AI --> A1[African Language AI]
 AI --> A2[AI Tutor]
 AI --> A3[AgroAI]
 AI --> A4[MedAI]
 AI --> A5[Knowledge Engine]
```

## Dépendances conceptuelles

```mermaid
flowchart LR
 DATA[Data & Evidence] --> AI[Applied AI]
 DATA --> CY[Cybersecurity]
 WEB[Web Infrastructure] --> DATA
 WEB --> SERVICES[Services utilisateurs]
 CY --> TRUST[Trust & Safety]
 AI --> SERVICES
 TRUST --> SERVICES
```

## Principe d'exécution

Chaque projet suit le même modèle :

1. Identifier un problème réel.
2. Documenter les utilisateurs et le contexte.
3. Vérifier les hypothèses avec des personnes concernées.
4. Construire le plus petit prototype utile.
5. Tester sur le terrain.
6. Mesurer l'impact et les effets indésirables.
7. Documenter ce qui fonctionne et ce qui échoue.
8. Publier, maintenir ou arrêter sur la base des résultats.

## Relations avec les missions

Les issues et missions du programme Contributor doivent pointer vers un dépôt projet lorsqu'elles demandent une contribution technique ou métier. Les missions transversales restent dans `hashcode-contributors`.

## Liens

- Programme Contributor : https://github.com/HashCode-Reboot/hashcode-contributors
- Catalogue Global Impact : [projets-impact-global.md](projets-impact-global.md)
