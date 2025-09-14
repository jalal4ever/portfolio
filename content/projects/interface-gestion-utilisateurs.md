---
title: "Gestion du cycle de vie des utilisateurs : une interface web tout-en-un"
description: "Automatiser la création, modification et suppression des utilisateurs via une interface centralisée, intégrant Active Directory, Entra ID, SharePoint et Microsoft 365"
dateString: Fev - Sep 2025
draft: false
tags: ["Active Directory", "Entra ID", "PowerShell", "Python", "SharePoint", "Automatisation", "Microsoft 365"]
showToc: false
weight: 201
cover:
    image: "projects/interface-gestion-utilisateurs/Cover.png"
---

# Pourquoi ce projet ?
Dans une entreprise, gérer le cycle de vie des utilisateurs — de leur arrivée à leur départ — est un processus fastidieux et source d’erreurs. Entre la création de comptes, l’attribution de licences, la gestion des groupes et la désactivation des accès, les administrateurs passent des heures sur des tâches répétitives. **Et si tout cela pouvait se faire en quelques clics, avec une validation humaine à chaque étape critique ?**
Cette interface web est née pour **réconcilier automatisation et contrôle**, en offrant une solution centralisée qui s’appuie sur les données RH, Active Directory, Entra ID et SharePoint.

---

# Boîte à outils : l’alliance de la puissance et de la simplicité
Pour construire cette solution, j’ai combiné :
- **PowerShell** et **Python** : le couteau suisse de l’automatisation, pour interagir avec Active Directory, Entra ID et Microsoft 365,
- **SharePoint** : la source de vérité pour les données RH, interrogée en temps réel,
- **Une interface web intuitive** : conçue pour les administrateurs, sans nécessiter de compétences en script,
- **Des notifications intelligentes** : pour alerter en cas d’anomalie ou de besoin d’intervention.

L’objectif ? **Transformer un processus complexe en un flux fluide et sécurisé.**

---

# À quoi s’attendre
## 1. Création d’un utilisateur
- L’interface lit les entrées depuis SharePoint (fichier RH ou saisie manuelle),
- Elle crée automatiquement le compte dans **Active Directory local** et **Entra ID**,
- Elle attribue les **licences Microsoft 365** adaptées au poste,
- Elle affecte l’utilisateur aux **groupes de sécurité** correspondants,
- Elle vérifie et suggère l’affectation d’un ordinateur, en croisant les données disponibles.

## 2. Modification d’un utilisateur
- Changement de nom, de fonction ou de service ? L’interface propose les modifications nécessaires,
- L’administrateur peut valider ou ajuster directement depuis le tableau de bord,
- Les mises à jour sont répercutées en temps réel dans **AD, Entra ID et SharePoint**.

## 3. Fin de contrat
- L’interface génère un **rapport complet** pour la RH (accès, licences, matériel),
- Elle désactive les comptes et supprime les accès selon les règles métiers,
- Elle propose une **vérification finale** avant suppression définitive.

---

# Un quotidien simplifié pour les administrateurs
Imaginez un tableau de bord où :
- Les **nouveaux utilisateurs** sont créés en 2 clics,
- Les **modifications** sont suggérées et appliquées après validation,
- Les **fin de contrat** sont gérées sans rien oublier,
- Les **ordinateurs orphelins** (sans utilisateur attribué) sont identifiés et proposés à la réaffectation.

**Plus de risques d’oubli, plus de tâches manuelles fastidieuses.** Juste une interface qui travaille pour vous, comme un assistant infatigable. ☕💻

---
Le saviez-vous ?
> L’interface vérifie aussi la cohérence des données entre SharePoint et Active Directory. Si un utilisateur existe dans l’un mais pas dans l’autre, elle alerte l’administrateur pour éviter les incohérences.

---

# Résultats concrets
- **Gain de temps** : jusqu’à 80 % de tâches automatisées,
- **Réduction des erreurs** : plus de comptes orphelins ou de licences inutiles,
- **Traçabilité** : un historique complet de toutes les actions,
- **Sérénité** : les administrateurs gardent la main sur les décisions critiques.

---
# Et demain ?
Cette interface est conçue pour évoluer : intégration avec d’autres outils (comme Ivanti ou ServiceNow), gestion des appareils mobiles, ou même un portail utilisateur pour les demandes simples. **L’automatisation n’a pas de limite !**

---
J’espère que ce projet vous inspirera pour vos propres défis d’automatisation. Si vous voulez en savoir plus ou échanger sur des cas d’usage similaires, n’hésitez pas à me contacter !
