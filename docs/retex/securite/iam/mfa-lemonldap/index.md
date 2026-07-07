
# RETEX – Reprise et sécurisation d’un projet MFA avec LemonLDAP

## Résumé

Ce retour d’expérience porte sur la reprise d’un projet de mise en œuvre de l’authentification multifacteur avec LemonLDAP.

Le projet répondait à un besoin fort de conformité et de sécurisation des accès aux applications critiques exposées ainsi qu’au Bureau Retraite.

La principale difficulté n’a pas été uniquement technique. Elle a surtout porté sur la reprise d’un sujet insuffisamment cadré, avec un calendrier déjà imposé, des dépendances techniques mal stabilisées et des ressources d’architecture non affectées.

---

## Contexte

Le projet visait à déployer une authentification forte sur plusieurs périmètres critiques.

Le sujet avait déjà connu une phase de préparation, mais sans cadrage opérationnel suffisamment robuste. Lorsque le projet a été repris, plusieurs éléments structurants restaient à stabiliser :

- jalons peu justifiés ;
- hypothèses d’architecture encore mouvantes ;
- dépendances techniques mal identifiées ;
- besoin de développements spécifiques non prévus, ajout de la monté de version France connect V2 ;
- absence des ressources d’architecture initialement demandées.

---

## Enjeux

Les principaux enjeux étaient les suivants :

- répondre aux exigences de conformité ;
- renforcer la sécurité des applications critiques ;
- tenir un calendrier imposé ;
- éviter toute interruption de service ;
- coordonner des acteurs techniques multiples sans appui hiérarchique fort.

---

## Rôle tenu

Le rôle exercé a dépassé le pilotage projet classique.

Il a combiné plusieurs dimensions :

- responsable de projet ;
- orchestrateur transverse ;
- coordinateur des équipes sécurité, infrastructure, exploitation et applicatives ;
- architecte de facto sur certains sujets ;
- facilitateur dans la résolution des blocages.

Le projet a nécessité de faire avancer les travaux sans autorité hiérarchique directe, en s’appuyant sur des relais d’influence et sur une forte proximité opérationnelle avec les équipes.

---

## Schéma de synthèse

schema.svg

---

## Difficultés rencontrées

### Cadrage initial incomplet

Le projet avait été engagé sur la base d’un calendrier déjà fixé, mais avec un cadrage insuffisamment stabilisé.

Certaines hypothèses n’étaient pas assez documentées, notamment sur les zones d’implémentation, les dépendances d’infrastructure et les besoins de personnalisation.

### Développements hors périmètre

Des demandes de customisation sont apparues en cours de projet alors qu’elles n’étaient pas présentes dans le cahier des charges initial.

Cette situation a généré une tension supplémentaire, car aucune équipe de développement dédiée n’était clairement affectée.

### Dépendance à un sachant unique

Le projet dépendait fortement d’un expert unique sur certains sujets d’infrastructure, notamment les zones VLAN et le cycle de vie des environnements.

Cette dépendance a créé une fragilité décisionnelle, des changements d’orientation et une perte de temps significative.

### Absence d’appui hiérarchique fort

Le projet a dû avancer sans appui direct du N+1 ou du N+2.

La progression s’est donc appuyée davantage sur l’influence, les relais opérationnels et la résolution concrète des problèmes que sur l’autorité formelle.

---

## Changement de méthode

Le pilotage initial reposait sur un fonctionnement classique, avec des points hebdomadaires.

Ce mode n’était pas adapté au niveau d’incertitude et au nombre de blocages rencontrés.

Le dispositif a donc été transformé en mode task-force :

- points quotidiens ;
- traitement des blocages sous 24 heures ;
- arbitrages point à point ;
- coordination rapprochée des acteurs ;
- suivi opérationnel très court terme.

Ce changement de rythme a permis de remettre le projet en mouvement et de sécuriser la livraison.

---

## Résultats obtenus

Les principaux résultats obtenus sont les suivants :

- déploiement du MFA sur les applications critiques ciblées ;
- sécurisation de l’accès au Bureau Retraite ;
- respect du calendrier imposé (livré été 2025) ;
- livraison malgré l’absence de certaines ressources clés ;
- montée en compétence sur les sujets IAM, MFA, SSO et protocoles d’authentification.

---

## Enseignements

### 1. Un projet mal cadré doit d’abord être diagnostiqué

Lorsqu’un projet est repris en cours de route, il ne faut pas se contenter d’exécuter le planning existant.

Il faut rapidement identifier :

- les hypothèses implicites ;
- les dépendances réelles ;
- les risques non visibles ;
- les acteurs clés ;
- les points de fragilité.

### 2. Le reporting ne suffit pas à redresser un projet

Un projet en difficulté ne se redresse pas par davantage de comités ou de reporting.

Il se redresse par :

- la proximité terrain ;
- le traitement rapide des blocages ;
- la clarification des responsabilités ;
- la réduction du temps entre problème et décision.

### 3. Les SPOF doivent être traités dès le démarrage

La dépendance à un sachant unique constitue un risque majeur.

Elle doit être identifiée dès les premières semaines et faire l’objet d’un plan de sécurisation.

### 4. L’influence peut compenser l’absence d’autorité

Même sans appui hiérarchique fort, il est possible de faire avancer un sujet complexe en s’appuyant sur :

- des relais fiables ;
- une compréhension fine des acteurs ;
- une capacité à rendre les problèmes visibles ;
- une animation opérationnelle régulière.

### 5. La reconnaissance ne suit pas toujours la contribution

Ce projet a également rappelé que la contribution réelle à la réussite d’un sujet n’est pas toujours visible spontanément.

Il est donc nécessaire de documenter, tracer et rendre lisible la valeur produite.

---

## Ce que je referais différemment

Si ce type de projet devait être repris aujourd’hui, les actions suivantes seraient engagées dès le démarrage :

- réaliser un diagnostic flash ;
- cartographier les dépendances critiques ;
- identifier les sachants uniques ;
- challenger les jalons de manière factuelle ;
- qualifier les besoins de développement ;
- installer plus tôt un mode task-force si le niveau d’incertitude est élevé.

---

