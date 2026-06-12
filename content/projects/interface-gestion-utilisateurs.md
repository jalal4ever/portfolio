```markdown
---
title: "Industrialisation du parcours utilisateurs : de PowerShell à Python"
description: "Refonte complète du processus de gestion des entrées et sorties utilisateurs afin d'améliorer la fiabilité, la maintenabilité et la standardisation des opérations IT."
dateString: 2025 - 2026
draft: false
tags: ["Python", "PowerShell", "Microsoft 365", "Automatisation", "Active Directory", "Entra ID", "Git", "SharePoint"]
showToc: false
weight: 201
cover:
    image: "projects/parcours-utilisateurs/Cover.png"
---

# Pourquoi ce projet ?

La gestion du cycle de vie des utilisateurs représente un enjeu majeur pour toute équipe IT.

Création de comptes, attribution de licences, affectation de matériel, gestion des arrivées et des départs : ces opérations doivent être réalisées rapidement tout en garantissant la cohérence des données, la sécurité des accès et la traçabilité des actions.

Historiquement, ces traitements reposaient sur plusieurs scripts PowerShell indépendants. Bien que fonctionnels, leur maintenance devenait de plus en plus complexe avec l'évolution des besoins et la multiplication des dépendances.

Afin de fiabiliser le processus et de préparer les futures évolutions, une refonte complète de l'architecture a été engagée autour d'une approche centralisée basée sur Python.

---

# Une nouvelle architecture pensée pour la fiabilité

L'objectif n'était pas simplement de réécrire les scripts existants, mais de construire une plateforme d'automatisation capable d'évoluer dans le temps.

Le nouveau modèle repose sur plusieurs principes :

- Un script orchestrateur centralisé.
- Des modules Python spécialisés pour chaque fonction métier.
- Une gestion indépendante des dépendances grâce aux environnements virtuels Python.
- Un stockage centralisé des configurations.
- Une distribution contrôlée des versions.

Cette architecture permet d'améliorer la stabilité des traitements tout en simplifiant leur maintenance.

---

# Des environnements Python isolés

L'une des difficultés rencontrées avec l'approche historique concernait la gestion des modules PowerShell et leurs différentes versions.

Le nouveau système s'appuie sur des environnements virtuels Python dédiés afin d'isoler les dépendances et garantir un fonctionnement identique sur chaque poste d'administration.

Cette approche permet :

- D'éliminer les conflits entre versions de modules.
- De simplifier les mises à jour.
- D'assurer la reproductibilité des environnements.
- De sécuriser les déploiements.

Chaque administrateur dispose ainsi du même environnement d'exécution et des mêmes versions de composants.

---

# Un orchestrateur centralisé

Au cœur de la solution se trouve un orchestrateur Python qui pilote l'ensemble des opérations.

Plutôt que d'exécuter localement des scripts dispersés, l'orchestrateur récupère automatiquement les modules depuis le dépôt Git de l'équipe.

Cette approche garantit :

- L'utilisation de la dernière version validée.
- La centralisation du code.
- Une meilleure gouvernance des évolutions.
- Une réduction des écarts entre les environnements.

Les paramètres et fichiers de configuration sont quant à eux centralisés sur SharePoint afin de disposer d'une source unique de configuration pour l'ensemble des administrateurs.

---

# Gestion des arrivées

L'orchestrateur centralise les opérations liées à l'intégration des nouveaux collaborateurs.

Depuis une interface unique, il est possible de :

- Créer les comptes utilisateurs.
- Attribuer les licences Microsoft 365.
- Configurer les signatures électroniques Letsignit.
- Affecter les groupes et habilitations nécessaires.
- Associer le matériel informatique au collaborateur.
- Garantir la cohérence des informations entre les différents systèmes.

L'ensemble du processus est standardisé afin de réduire les interventions manuelles et les risques d'erreur.

---

# Gestion des départs

Le projet couvre également l'ensemble du processus de sortie des collaborateurs.

L'outil permet notamment de :

- Identifier les comptes et accès associés.
- Recenser les licences attribuées.
- Consulter le matériel affecté à l'utilisateur.
- Suivre la restitution des équipements.
- Préparer les opérations de désactivation et d'archivage.

Cette visibilité facilite le travail des équipes IT tout en améliorant la traçabilité des restitutions.

---

# Synchronisation avec les données RH

La qualité des données constitue un élément essentiel du dispositif.

L'orchestrateur intègre un mécanisme de synchronisation permettant de comparer régulièrement les informations présentes dans le système d'information avec celles issues des référentiels RH.

Cette démarche permet :

- De détecter les écarts de données.
- De corriger les incohérences.
- De maintenir une information fiable.
- De renforcer la qualité des processus d'administration.

L'objectif est de disposer en permanence d'une vision cohérente et à jour des utilisateurs et de leurs affectations.

---

# Résultats obtenus

Cette refonte a permis de transformer un ensemble de scripts indépendants en une solution cohérente et évolutive.

Les principaux bénéfices sont :

- Une standardisation des opérations d'administration.
- Une meilleure maîtrise des versions déployées.
- Une réduction des problèmes liés aux dépendances techniques.
- Une amélioration de la qualité des données.
- Une simplification de la gestion des arrivées et des départs.
- Une meilleure traçabilité des actions réalisées.
- Une base solide pour les futures automatisations.

Au-delà du gain opérationnel, ce projet illustre une démarche d'industrialisation des processus IT visant à rendre les opérations plus fiables, plus maintenables et plus sécurisées.
```
