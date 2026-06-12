---
title: "Gestion du cycle de vie des utilisateurs : automatisation des processus IT"
description: "Centraliser et automatiser les opérations de création, modification et départ des collaborateurs dans un environnement Active Directory hybride."
dateString: Fev - Sep 2025
draft: false
tags: ["Active Directory", "Entra ID", "PowerShell", "Python", "Microsoft 365", "Automatisation", "Identity Management"]
showToc: false
weight: 201
cover:
    image: "projects/interface-gestion-utilisateurs/Cover.png"
---

# Contexte

Dans un environnement hybride combinant Active Directory, Entra ID et Microsoft 365, la gestion du cycle de vie des utilisateurs représente une part importante des opérations d'administration.

Les arrivées, changements de poste et départs nécessitent de nombreuses actions : création des comptes, affectation des groupes de sécurité, attribution des licences Microsoft 365, gestion des équipements et suppression des accès.

Afin de réduire les tâches manuelles, fiabiliser les traitements et améliorer la traçabilité, j'ai développé une interface web centralisant l'ensemble de ces opérations.

---

# Objectifs du projet

Cette solution répond à plusieurs enjeux :

- Standardiser les processus d'administration des identités.
- Réduire les erreurs liées aux opérations manuelles.
- Améliorer la traçabilité des actions réalisées.
- Garantir l'application des règles de gestion définies par la DSI.
- Simplifier les opérations quotidiennes des administrateurs.

---

# Technologies utilisées

L'application repose sur plusieurs briques techniques :

- PowerShell pour les interactions avec Active Directory, Microsoft 365 et Entra ID.
- Python pour les traitements métiers et l'interface applicative.
- Active Directory comme référentiel principal des identités.
- Entra ID pour les services cloud Microsoft 365.
- SharePoint pour le stockage et le suivi des demandes administratives.
- API Microsoft Graph pour certaines opérations cloud.

---

# Fonctionnalités principales

## Gestion des arrivées

Lors de l'intégration d'un collaborateur, l'application permet :

- La création automatique du compte Active Directory.
- L'application des conventions de nommage définies par l'entreprise.
- L'affectation des groupes de sécurité selon le métier ou le service.
- L'attribution des licences Microsoft 365 nécessaires.
- Le déclenchement des processus de synchronisation vers Entra ID.
- La génération d'un compte-rendu des actions réalisées.

## Gestion des modifications

L'interface centralise les demandes de changement :

- Modification des informations utilisateur.
- Changement de service ou de fonction.
- Mise à jour des groupes et habilitations.
- Réattribution ou ajustement des licences Microsoft 365.
- Historisation des modifications effectuées.

## Gestion des départs

Lorsqu'un collaborateur quitte l'entreprise :

- Désactivation du compte Active Directory.
- Révocation des accès Microsoft 365.
- Retrait des groupes et habilitations.
- Inventaire des licences à récupérer.
- Génération d'un rapport destiné aux équipes IT et RH.
- Conservation des informations conformément aux procédures internes.

---

# Contrôles et cohérence des données

L'application intègre plusieurs mécanismes de contrôle :

- Vérification de l'existence des comptes dans Active Directory et Entra ID.
- Détection des incohérences entre les différentes sources de données.
- Contrôle des licences attribuées.
- Identification des équipements non affectés.
- Journalisation complète des opérations réalisées.

---

# Bénéfices obtenus

La mise en place de cette solution a permis :

- Une réduction significative du temps consacré aux tâches récurrentes.
- Une meilleure homogénéité des configurations utilisateurs.
- Une diminution des erreurs de saisie et d'attribution.
- Une amélioration de la traçabilité des opérations administratives.
- Une meilleure maîtrise du cycle de vie des identités.

---

# Perspectives d'évolution

Plusieurs évolutions sont envisagées :

- Intégration avec un outil ITSM.
- Automatisation des workflows de validation.
- Gestion avancée des équipements.
- Intégration avec les solutions MDM et EMM.
- Mise en place de tableaux de bord de suivi et de reporting.

---

Ce projet illustre comment l'automatisation peut contribuer à renforcer la qualité de service de la DSI tout en conservant les mécanismes de contrôle nécessaires à la gestion des identités et des accès.
