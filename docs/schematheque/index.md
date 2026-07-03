
# Schémathèque

## Objectif

La schémathèque rassemble les schémas, cartographies, modèles et représentations visuelles utilisés dans le cadre de la gouvernance technique, de l'architecture, de l'exploitation et du pilotage des projets.

Chaque fiche est composée de :

- Un schéma (SVG, Mermaid ou PowerPoint).
- Une description de l'objectif.
- Une lecture rapide.
- Une représentation textuelle.
- Les concepts, protocoles ou standards associés.
- Les points d'attention et bonnes pratiques.

---

## Catégories

### Réseau

Documentation des couches réseau, protocoles et infrastructures de communication.

- [Couches, composantssants-standards/

---

### Sécurité

Documentation des mécanismes d'authentification, de chiffrement et de contrôle d'accès.

*À compléter*

---

### IAM (Identity & Access Management)

Documentation des annuaires, fédérations d'identité et solutions SSO.

*À compléter*

---

### Middleware

Documentation des bus d'événements, solutions d'intégration et échanges inter-applicatifs.

*À compléter*

---

### Cloud & Kubernetes

Documentation des architectures cloud, conteneurs et plateformes Kubernetes.

*À compléter*

---

### Observabilité

Documentation des solutions de supervision, métrologie, logs et traçabilité.

*À compléter*

---

### Architecture d'entreprise

Cartographies fonctionnelles, applicatives et techniques.

*À compléter*

---

### Gouvernance

Supports visuels utilisés pour le pilotage, les comités et les démarches de gouvernance.

*À compléter*

---

## Convention utilisée

Chaque schéma est stocké dans un répertoire dédié :

```text
schematheque/
└── categorie/
    └── nom-du-schema/
        ├── index.md
        ├── schema.svg
        └── schema.yaml
```

### Exemple

```text
schematheque/
└── reseau/
    └── couches-composants-standards/
        ├── index.md
        ├── schema.svg
        └── schema.yaml
```

---

## Public cible

Cette schémathèque s'adresse notamment à :

- Architectes
- Chefs de projet techniques
- Responsables d'exploitation
- Équipes infrastructure
- Équipes sécurité
- PMO et gouvernance
- Nouveaux arrivants souhaitant comprendre le SI

---

## Principes

- Favoriser les représentations visuelles simples.
- Associer systématiquement une explication textuelle.
- Utiliser un vocabulaire compréhensible par le plus grand nombre.
- Capitaliser les retours d'expérience.
- Maintenir les schémas sous forme éditable lorsque cela est possible.

---

> Une image vaut mille mots, à condition qu'elle soit comprise de la même façon par tous.

