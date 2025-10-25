*Ce document résume les idées et les réflexions majeures issues de la discussion par mail entre Hilaire Fernandes (porteur du projet Dybo) et Georges (enseignant retraité) en avril 2023.*

***

# Synthèse Détaillée : Échange Dybo (Hilaire Fernandes et Georges)

Ce document résume les idées et les réflexions majeures issues de la discussion par mail entre Hilaire Fernandes (porteur du projet Dybo) et Georges (enseignant retraité).

***

## 1. Vision et Philosophie du Projet Dybo

| Idée Clé | Détails et Objectifs |
| :--- | :--- |
| **Philosophie Fondatrice** | Dybo est un **système informatique nomade libre** (**hardware et logiciel**), centré sur le principe du **logiciel libre** dont le code source est poussé jusqu'à l'utilisateur final. |
| **Objectif Pédagogique** | Remplacer les trois principaux supports de l'élève : **les livres, les cahiers et les classeurs**. |
| **Point de Départ** | Le développement est initié par la fonction essentielle de la **prise de note manuscrite** (pour remplacer le cahier). |
| **Durabilité** | Le matériel doit être conçu pour une durée de vie de **8 à 9 ans**, couvrant le parcours scolaire du CM1/CM2 à la Terminale. |

***

## 2. Conception Matérielle et Technique (Hardware)

| Idée Clé | Spécifications et Justifications |
| :--- | :--- |
| **Format Physique** | Un appareil de la taille d'un **grand cahier**, légèrement supérieur au format A4. |
| **Écrans et Stylet** | **Deux écrans A4** (ou 14-15 pouces) sont nécessaires pour permettre aux élèves de travailler confortablement avec **deux documents simultanément** (ex: manuel et cahier). L'utilisation d'un **stylet** est fondamentale pour la prise de notes manuscrites. |
| **Poids et Ergonomie** | Puisque Dybo remplace **8 à 10 kg** de fournitures scolaires, un poids de **3 ou 4 kg** est jugé acceptable. Georges suggère cependant que **2,5 kg** serait un poids plus convaincant pour faciliter l'adoption. |
| **Architecture** | Le choix se porte sur un processeur **"libre" RISC V** et un système d'exploitation **Linux** (idéalement en Framebuffer). |

***

## 3. Conception Logicielle et Pédagogique

| Idée Clé | Fonctionnalités et Concepts |
| :--- | :--- |
| **Modèle Pédagogique** | Basé sur le concept du **Modèle Informatisé de Connaissance** (*dynamic media*) d'Alan Kay. |
| **Le Cahier Numérique** | Le logiciel principal, **PaperMorph**, est la **colonne vertébrale** qui simule le cahier de l'élève. Il gère l'insertion de **notes manuscrites** et de **médias dynamiques** (*Morphs*). |
| **Appropriation par le Libre** | Les **médias dynamiques** doivent être **facilement modifiables** par les enseignants néophytes pour favoriser une montée en compétence et l'adhésion à la philosophie libre. |
| **Fonctions "Métier"** | Le logiciel intègre les pratiques de l'enseignement : ouverture automatique du **classeur ad-hoc** selon l'horaire, proposition d'**agender** automatiquement un travail donné, gestion des documents **PDF** avec annotation au stylet. |

***

## 4. Ressources Pédagogiques Associées

| Idée Clé | Contexte et Modèles Cités |
| :--- | :--- |
| **Situation en France** | Plusieurs associations professionnelles d'enseignants développent des manuels scolaires libres. Voir ce qui est possible avec l'éditeur pédagogique national (CANOPE), mais **ce domaine semble réservé au privé. |
| **Gestion des PDF** | Le Dybo doit pouvoir gérer les documents **PDF** (libres ou non) et permettre leur **annotation au stylet** et leur **partage** entre élèves et enseignants. |
| **Modèle de Genève** | Le modèle du **Canton de Genève** est cité comme un exemple de réussite, car les **enseignants produisent la majorité des ressources** eux-mêmes. Cela valide une approche décentralisée de la création de contenu. |

***

## 5. Évaluation et Interactivité (Scénario AMC)

| Idée Clé | Application et Avantages de l'Auto-Correction |
| :--- | :--- |
| **Lien Logiciel** | Dybo est adapté à l'utilisation du logiciel **Auto-Multiple-Choice (AMC)**. |
| **Correction Instantanée** | Le Dynabook de l'enseignant **corrige automatiquement** le travail rendu par les élèves (via onde locale), enregistre la note et renvoie le corrigé à l'élève, tout cela en **moins de 15 secondes**. |
| **Avantages** | Le scénario **élimine le besoin de photocopie et de scan** pour l'évaluation et permet des interactions pédagogiques impossibles avec le papier (ex : QCM randomisés). |

***

## 6. Connectivité et Défis de Déploiement

| Idée Clé | Problèmes Soulevés et Solutions Dybo |
| :--- | :--- |
| **Réseau Wi-Fi Institutionnel** | Constat de la **médiocrité et de la non-fiabilité** des réseaux Wi-Fi des établissements (problèmes de bornes/Radius). |
| **Solution Dybo (Autonomie)** | L'utilisation en classe **ne doit pas nécessiter d'authentification distante**. Le partage de documents se fait **localement en classe de pair à pair** via **Bluetooth et/ou Wi-Fi** depuis le Dynabook de l'enseignant. Un **réseau local Wi-Fi est la bonne solution**. |
| **Stratégie d'Adoption** | L'approche doit être **humble** et permettre à Dybo de **cohabiter avec les usages traditionnels**. L'utilisateur doit en tirer un **bénéfice individuel, visible et mesurable**. |
| **Scénarios de Déploiement** | **Approche "Par le Haut"** (établissement entier nécessitant une "volonté politique crédible") ou **Approche "Par le Bas"** (petite équipe pédagogique dans un établissement ordinaire, jugée plus fréquente). |
