# 🎓 Cas Pratique : Optimisation du Processus de Gestion des Commandes d'une PME e-Commerce

## 📌 Contexte Général

Une PME vend des produits électroniques en ligne via un site web. Elle gère tout en interne : commandes, stock, facturation et livraisons. Le directeur remarque :

* Des **retards fréquents** de livraison.
* Des **erreurs de stock**.
* Des **clients insatisfaits**.
* Un **manque de traçabilité** dans le traitement des commandes.

Il souhaite **digitaliser** et **automatiser** les processus avec une solution plus intégrée.

---

## 🎯 Objectif du Cas Pratique

**En tant que Business Analyst**, tu dois :

1. Analyser le processus existant.
2. Identifier les points de blocage.
3. Proposer une solution fonctionnelle et technologique.
4. Modéliser les processus.
5. Élaborer un backlog Agile.
6. Définir des indicateurs de performance.
7. Proposer une stratégie d’évolution à 6-12 mois.

---

## 🧩 Étapes du Cas Pratique

---

### 1. 🗺️ Analyse du processus actuel (As-Is)

#### 🔍 Étude documentaire :

* Site e-commerce simple, sans ERP ni CRM.
* Utilisation d’un fichier Excel pour gérer les commandes.
* Paiements via PayPal, sans synchronisation avec la gestion des stocks.
* Suivi des livraisons manuel par mail.

#### 📌 Processus actuel (simplifié) :

1. Client commande via le site.
2. Mail envoyé au gestionnaire.
3. Commande saisie dans Excel.
4. Stock vérifié manuellement.
5. Livraison déclenchée si produit dispo.
6. Facture manuelle + envoi au client.

#### 🛑 Problèmes identifiés :

* Risque d’erreurs (copie manuelle)
* Pas de validation de stock automatique
* Aucun lien entre la commande, le stock, et la livraison
* Pas de tableau de bord ou de KPIs
* Service client débordé de relances

---

### 2. 📈 Représentation du processus (BPMN)

> Outil suggéré : **Bizagi Modeler** ou **Draw\.io**

Créé un diagramme BPMN représentant ce flux :

* Début (commande)
* Vérification stock
* Saisie manuelle dans Excel
* Livraison ou annulation
* Envoi de facture

---

### 3. 📊 Recommandations & Solution cible (To-Be)

#### 🛠️ Proposition de Solution :

Implémenter un système de gestion intégré :

* **ERP open source (ex : Odoo, Dolibarr, ERPNext)**
* Module e-commerce + gestion des stocks + facturation + CRM
* Synchronisation automatique site ↔ ERP
* Dashboard de suivi + automatisation des tâches

#### ✅ Objectifs visés :

* Réduction des erreurs
* Amélioration des délais de livraison
* Meilleur suivi client
* Vision en temps réel du stock et des ventes

---

### 4. 📚 Cahier des charges fonctionnel

#### Extrait :

| Fonctionnalité        | Description                                                |
| --------------------- | ---------------------------------------------------------- |
| Gestion des commandes | Saisie automatique depuis le site web                      |
| Suivi des stocks      | Décrément automatique à la commande                        |
| Facturation           | Génération automatique à la validation                     |
| Dashboard             | Indicateurs : stock critique, commandes en attente, délais |
| CRM                   | Historique client, tickets, préférences                    |

---

### 5. 🏗️ Modèle de données simplifié

| Entité    | Attributs                              |
| --------- | -------------------------------------- |
| Client    | ID, Nom, Email, Adresse                |
| Commande  | ID, Date, État, Montant, Client\_ID    |
| Produit   | ID, Nom, Stock, Prix                   |
| Facture   | ID, Commande\_ID, Montant, Statut      |
| Livraison | ID, Commande\_ID, Transporteur, Statut |

---

### 6. 🪃 Backlog Agile (format user stories)

| ID    | User Story                                                                             |
| ----- | -------------------------------------------------------------------------------------- |
| US001 | En tant que client, je veux recevoir un mail de confirmation après ma commande         |
| US002 | En tant que gestionnaire, je veux être notifié d’un stock faible pour réapprovisionner |
| US003 | En tant qu’admin, je veux consulter un dashboard des commandes en attente              |
| US004 | En tant que comptable, je veux pouvoir exporter les factures au format PDF             |
| US005 | En tant que client, je veux suivre mon colis depuis mon espace personnel               |

---

### 7. 📏 Indicateurs de performance (KPIs)

| KPI                                | Objectif    |
| ---------------------------------- | ----------- |
| Taux d’erreur de stock             | < 1%        |
| Délai moyen de livraison           | < 3 jours   |
| Satisfaction client                | > 85%       |
| Taux de commande annulée           | < 2%        |
| Temps moyen de traitement commande | < 5 minutes |

---

### 8. 🧠 Éléments de stratégie IT (court et moyen terme)

#### Court terme (3-6 mois) :

* Implémenter Odoo ou ERPNext.
* Connecter le site e-commerce à l’ERP.
* Former les utilisateurs.

#### Moyen terme (6-12 mois) :

* Ajouter module CRM.
* Mettre en place un chatbot.
* Intégrer une BI pour analyse des ventes.

---

### 9. 📝 Livrables attendus

* BPMN du processus actuel et cible
* Cahier des charges fonctionnel (10 à 15 pages)
* Table de mapping des données (modèle relationnel)
* Backlog Agile (au moins 10 user stories)
* Maquettes d’interface (Figma, Balsamiq)
* Présentation PowerPoint synthétique
* Rapport final avec recommandations stratégiques

---

## 📂 Bonus : Structure de Dossier (Portfolio)

```
/cas_pratique_gestion_commandes/
├── 01_context_contexte_general.pdf
├── 02_processus_bpmn_as_is_to_be.drawio
├── 03_cahier_des_charges.pdf
├── 04_modele_donnees.xlsx
├── 05_user_stories_backlog.xlsx
├── 06_kpi_dashboard.xlsx
├── 07_maquettes_interface_figma.png
├── 08_plan_strategique_it.pdf
├── 09_presentation_finale.pptx
```

---

## ✅ Conclusion

Ce cas pratique t'offre une **expérience complète**, depuis l’analyse métier jusqu’à la proposition d’une stratégie IT réaliste. Il te permet de mettre en œuvre tes compétences et de créer **des livrables concrets** pour ton **portfolio professionnel**.

Souhaites-tu que je te génère certains fichiers types (BPMN, backlog, maquettes ou présentation PowerPoint) pour t’aider à démarrer ?
