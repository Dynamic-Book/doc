*Ce document résume les idées et les réflexions majeures issues de la discussion par mail entre Hilaire Fernandes (porteur du projet Dybo) et Georges (enseignant retraité) en avril 2023.*

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
| **Poids et Ergonomie** | Puisque Dybo remplace **8 à 10 kg** de fournitures scolaires, un poids de **3 ou 4 kg** est jugé acceptable. Cependant, Georges suggère qu'un poids de **2,5 kg** serait plus convaincant pour faciliter l'adoption et l'éviter comme "barrière de potentiel". |
| **Architecture** | Le choix se porte sur un processeur **"libre" RISC V** et un système d'exploitation **Linux** (idéalement en Framebuffer). |
| **Connectique** | L'appareil doit être capable de gérer la connectivité **sans fil localisée** (voir point 5) pour un fonctionnement autonome en classe. |

***

## 3. Conception Logicielle et Pédagogique

| Idée Clé | Fonctionnalités et Concepts |
| :--- | :--- |
| **Modèle Pédagogique** | Basé sur le concept du **Modèle Informatisé de Connaissance** (*dynamic media*) d'Alan Kay. |
| **Le Cahier Numérique** | Le logiciel principal, **PaperMorph**, est la **colonne vertébrale** simulant le cahier de l'élève. Il gère l'insertion de **notes manuscrites** et de **médias dynamiques** (*Morph*). |
| **Appropriation par le Libre** | Les **médias dynamiques** sont fournis via des bibliothèques de scripts. Ils doivent être **facilement modifiables** par les enseignants néophytes pour favoriser une montée en compétence (lien avec la philosophie libre). |
| **Fonctions "Métier"** | Le logiciel intègre les pratiques de l'enseignement : ouverture automatique du **classeur ad-hoc** selon l'horaire, proposition d'**agender** automatiquement un travail, gestion des documents **PDF** avec annotation au stylet. |

***

## 4. Évaluation et Interactivité (Scénario AMC)

| Idée Clé | Application et Avantages de l'Auto-Correction |
| :--- | :--- |
| **Lien Logiciel** | Dybo est adapté à l'utilisation du logiciel **Auto-Multiple-Choice (AMC)** (maintenu par Georges via un paquet Debian). |
| **Scénario d'Évaluation** | L'enseignant envoie un document de travail **AMC** aux élèves par **onde locale** (Wi-Fi/Bluetooth). |
| **Correction Instantanée** | Les élèves rendent le document à l'enseignant, dont le Dynabook **corrige automatiquement**, enregistre la note et renvoie le travail corrigé à l'élève, le tout en **moins de 15 secondes**. |
| **Avantages** | Le scénario élimine le besoin de photocopie et de scan pour l'évaluation et permet des interactions pédagogiques impossibles avec le papier (ex : QCM randomisés). |

***

## 5. Connectivité et Défis de Déploiement

| Idée Clé | Problèmes Soulevés et Solutions Dybo |
| :--- | :--- |
| **Réseau Wi-Fi Institutionnel** | Constat de la **médiocrité et de la non-fiabilité** des réseaux Wi-Fi des établissements (problèmes de bornes/Radius) ayant mené à l'échec des dotations passées. |
| **Solution Dybo (Autonomie)** | L'utilisation en classe **ne doit pas nécessiter d'authentification distante**. Le partage de documents se fait **localement en classe de pair à pair** (Peer-to-Peer) via **Bluetooth et/ou Wi-Fi** depuis le Dynabook de l'enseignant. Un **réseau local Wi-Fi est la bonne solution** dans la majorité des cas. |
| **Stratégie d'Adoption** | L'approche doit être **humble** et permettre à Dybo de **cohabiter avec les usages traditionnels**. L'utilisateur doit en tirer un **bénéfice individuel, visible et mesurable**. |
| **Scénarios de Déploiement** | **Approche "Par le Haut"** (établissement entier nécessitant une "volonté politique crédible") ou **Approche "Par le Bas"** (petite équipe pédagogique dans un établissement ordinaire, jugée plus fréquente). |
| **Obstacles Institutionnels** | Le système français est jugé **auto-blocant** en raison du "mille-feuille pédagogique et administratif", de la friction entre prescripteurs et de l'interdiction faite à l'éditeur national d'éditer des manuels. |


