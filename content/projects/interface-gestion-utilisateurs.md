---

title: "Industrialisation du parcours utilisateurs : de PowerShell à Python"
description: "Conception d'une plateforme centralisée pour automatiser et fiabiliser la gestion du cycle de vie des utilisateurs au sein du système d'information."
dateString: 2025 - 2026
draft: false
tags: ["Python", "PowerShell", "Microsoft 365", "Automatisation", "Active Directory", "Entra ID", "Git", "SharePoint", "Letsignit"]
showToc: false
weight: 201
cover:
    image: "projects/interface-gestion-utilisateurs/Cover.png"

---

# Vue d'ensemble du projet

La gestion du cycle de vie des utilisateurs constitue un processus critique au sein du système d'information. Chaque arrivée, mobilité ou départ implique de nombreuses opérations nécessitant rigueur, cohérence et traçabilité.

Historiquement, ces opérations reposaient sur plusieurs scripts PowerShell indépendants permettant d'automatiser certaines tâches d'administration. Bien que performante à ses débuts, cette approche présentait progressivement certaines limites liées à la maintenance, à la gestion des dépendances et à l'homogénéité des versions utilisées par les administrateurs.

Dans une logique d'amélioration continue et de standardisation des pratiques, une refonte complète de la solution a été engagée afin de construire une plateforme centralisée capable d'accompagner durablement l'évolution des besoins de l'entreprise.

---

# Boîte à outils technologique : Python, Git et SharePoint

Cette nouvelle génération d'outils repose sur une architecture Python modulaire conçue pour améliorer la fiabilité, la maintenabilité et l'évolutivité des traitements.

L'écosystème s'appuie notamment sur :

* Python pour l'automatisation et l'orchestration des processus.
* Des environnements virtuels Python afin de garantir l'isolation des dépendances.
* Un dépôt Git centralisé assurant la gestion des versions et la diffusion des évolutions.
* SharePoint comme référentiel central de configuration.
* Active Directory et Microsoft Entra ID pour la gestion des identités.
* Microsoft 365 et Letsignit pour les services utilisateurs.

Cette approche garantit à chaque administrateur de travailler avec les mêmes versions de composants et les mêmes paramètres de configuration.

---

# Une architecture pensée pour la gouvernance

Au cœur du dispositif se trouve un orchestrateur centralisé capable de piloter l'ensemble des opérations métier.

Plutôt que de maintenir localement plusieurs scripts indépendants, l'orchestrateur récupère automatiquement les modules validés depuis le dépôt Git de l'équipe.

Cette architecture permet :

* D'assurer l'utilisation des dernières versions validées.
* De simplifier la maintenance des développements.
* D'améliorer la gouvernance des évolutions.
* De réduire les écarts entre les environnements d'administration.
* De faciliter l'intégration de nouvelles fonctionnalités.

Les fichiers de configuration sont quant à eux centralisés sur SharePoint afin de garantir une cohérence globale des paramétrages utilisés en production.

---

# À quoi s'attendre

La plateforme centralise l'ensemble des opérations liées au parcours utilisateur.

Depuis une interface unique, les administrateurs peuvent notamment :

* Créer les nouveaux collaborateurs.
* Modifier les informations existantes.
* Attribuer les licences Microsoft 365.
* Déployer automatiquement les signatures Letsignit.
* Affecter le matériel informatique.
* Gérer les groupes et habilitations.
* Contrôler les informations de référence.
* Préparer et suivre les départs des collaborateurs.

L'ensemble des traitements s'appuie sur des processus standardisés afin de garantir la cohérence des opérations et la qualité des données.

---

# Synchronisation et qualité des données

La fiabilité d'un système d'information repose avant tout sur la qualité de ses données.

Dans cette optique, la plateforme intègre des mécanismes de synchronisation permettant de rapprocher les informations issues des référentiels RH avec celles présentes dans les différents systèmes administrés.

Cette démarche permet :

* De détecter rapidement les écarts de données.
* De renforcer la cohérence des informations utilisateurs.
* D'améliorer la qualité des référentiels.
* De limiter les erreurs administratives.
* De sécuriser les processus d'entrée et de sortie.

L'objectif est de disposer d'une vision fiable et actualisée de chaque collaborateur tout au long de son parcours dans l'entreprise.

---

# Des opérations quotidiennes simplifiées

Imaginez un environnement où l'ensemble des actions liées au cycle de vie des utilisateurs est accessible depuis une interface unique, cohérente et standardisée.

Les arrivées sont préparées plus rapidement.
Les licences sont attribuées automatiquement.
Les signatures sont déployées sans intervention manuelle.
Les équipements sont suivis plus efficacement.
Les départs sont sécurisés et tracés.
Les données RH restent cohérentes avec les systèmes techniques.

Cette plateforme ne se limite pas à l'automatisation de tâches administratives. Elle constitue un véritable levier d'industrialisation des processus IT, permettant de gagner en fiabilité, en traçabilité et en qualité de service tout en préparant les futures évolutions du système d'information.
