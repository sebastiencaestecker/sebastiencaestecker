# Sébastien Caestecker – Résoudre des problèmes métier avec la data | SQL • Power BI • Python • GCP

## Je ne suis pas arrivé dans la data par amour des chiffres, mais par nécessité opérationnelle.

Pendant 10 ans chez Leclerc, j’ai vécu les vraies questions de terrain :

* Pourquoi les ventes ralentissent-elles sur une catégorie clé ? Pourquoi le panier moyen diminue-t-il au drive ?
* Comment limiter les ruptures en rayon sans surstocker inutilement ?
* Quels types de produits nos clients achètent-ils, et à quel moment ?
* Pourquoi un collaborateur pourtant performant envisage-t-il de partir ?
* Comment optimiser le parcours de préparation drive pour gagner en vitesse et en efficacité ?
* Comment adapter le budget en cours de route, pour améliorer la marge ?

Je n’avais pas tous les outils, mais une certitude :
* Si tu veux une réponse utile, commence par poser la bonne question. Ensuite, les données te diront quoi faire

C’est ce que je fais aujourd’hui, avec méthode et rigueur.

*  Je comprends les contraintes business parce que je les ai vécues.
*  Je vais droit au but : besoin clair, analyse juste, résultat qui fait bouger les choses.
*  Je travaille pour/avec les métiers pour prendre la meilleure décision, plus rapidement.

Je suis un analyste qui comprend le métier **avant** la donnée.
Un ex-manager qui parle le langage du terrain.
Et un **data solver**, capable de transformer un problème en un plan d’action.

**📌 Enjeux traités :**

* Ciblage client & campagnes CRM rentables
* Churn & onboarding dans un modèle freemium
* Analyse multi-magasins & logistique dernier km
* Pricing public équitable (secteur public)
* Rétention RH & performance des équipes

## 🛠️ Mes outils du quotidien

- **SQL** (BigQuery, Snowflake, PostgreSQL, SQL Server)
- **Power BI** (DAX, Power Query)
- **Python** (Pandas, Numpy)
- **Cloud** : GCP, Azure, Snowflake
- **Autres** : Excel, GitHub, Notion


🎯 Je cherche un poste de data analyst ou performance analyst où la donnée permet d’agir, pas juste de rapporter.

---


## 🌍 [Projets data orientés métier](https://github.com/sebastiencaestecker?tab=repositories)
Voici quelques exemples concrets de projets où j’ai utilisé la data pour résoudre des problèmes métier :  



### 📌 [Fidéliser les clients Silver via une campagne ciblée – Secteur : Retail / e-commerce](https://github.com/sebastiencaestecker/Ciblage_campagne_pour_booster_vente_saisonniere)

**🎯 Ciblage intelligent des clients Silver – RFM & ROI CRM**
* Objectif : Booster la fidélité et la valeur du segment Silver (RFM = 6/7) via une campagne ciblée sur une catégorie à forte marge.

**💡 Problème business :**
* Les clients Silver sont actifs mais achètent peu dans une catégorie stratégique : Outerwear & Coats (marge >55 %, panier moyen >150 €).
* Comment les inciter à acheter cette catégorie sous-consommée ?

**🧠 Solution apportée (100 % SQL sur BigQuery) :**

* Analyse SQL croisée RFM x catalogue produits sur BigQuery
* Identification des clients Silver n’ayant jamais acheté de manteaux
* Sélection d’un groupe exposé (1 673 clients) et témoin (147) via RAND()
* Simulation d’une campagne avec 25 € offerts dès 100 € d’achat
* Estimation ROI : x1.97 avant même le lancement

**📈 Résultats attendus :**

* +84 acheteurs potentiels
* CA estimé = 11 340 €
* Marge = 6 237 €
* Coût = 2 100 €
* ROI estimé = +97 %

**🧩 Compétences mobilisées :**
SQL avancé · Segmentation RFM · Construction de groupes témoins · Simulation ROI · Analyse produit x client

📌 Projet 100 % SQL – réalisé sur BigQuery avec le dataset public thelook_ecommerce

➡️ *[Voir le projet](https://github.com/sebastiencaestecker/Ciblage_campagne_pour_booster_vente_saisonniere)*


---

### 📌 [Segmenter sa base client par RFM – Secteur : Retail / e-commerce](https://github.com/sebastiencaestecker/Segmentation_RFM_SQL)

**🎯 Segmentation RFM Client – Cibler les bons clients**
* Aider une équipe CRM à **prioriser ses campagnes marketing** en segmentant les clients selon leur valeur réelle (dataset : `thelook_ecommerce`).

**💡 Problème business :**
* Comment concentrer les efforts marketing sur les clients les plus rentables, tout en identifiant les segments à activer, développer ou exclure ?*

**🧠 Solution apportée (100 % SQL sur BigQuery) :**

* Segmentation RFM complète (Récence, Fréquence, Montant d'achat)
* Scoring via `PERCENTILE_CONT()` pour découpage précis des quartiles
* Attribution d’un **statut client métier** : Platine, Gold, Silver, Bronze, Iron
* Analyse croisée CA / volume / panier moyen par segment
* Recommandations CRM opérationnelles pour chaque statut

**📊 Résultats :**

| Segment | % Clients | CA (€)    | Panier moyen | Insight CRM                |
| ------- | --------- | --------- | ------------ | -------------------------- |
| Platine | 16 %      | 215 543 € | 202 €        | Club VIP, pré-lancement    |
| Gold    | 21 %      | 200 889 € | 141 €        | Offres personnalisées      |
| Silver  | 30 %      | 144 117 € | 72 €         | Cross-sell, booster panier |
| Bronze  | 25 %      | 62 235 €  | 38 €         | Promotions simples         |
| Iron    | 7 %       | 8 461 €   | 19 €         | Réactivation ou exclusion  |


* 48 % du CA généré par 38 % des clients (Platine + Gold) → focus
* Segment Silver = fort levier de progression
* Segment Iron = effort inutile → à désactiver

**🧩 Compétences mobilisées:** SQL(GROUP BY, DATE_DIFF, PERCENTILE_CONT) · Segmentation RFM · BigQuery · performanace business · recommandation CRM

➡️ *[Voir le projet](https://github.com/sebastiencaestecker/Segmentation_RFM_SQL)*


---

### 📌 [Optimiser l’onboarding dans un modèle freemium – Secteur : SaaS / e-commerce](https://github.com/sebastiencaestecker/Optimiser-l-onboarding-client-pour-maximiser-les-conversions-dans-une-offre-freemium)  

**🎯 Objectif :**
Améliorer la conversion post-essai gratuit et réduire le churn dans un modèle freemium SaaS, en identifiant les parcours à risque et les plans à forte rétention.


**🧠 Problème métier :**

Comment transformer plus d’utilisateurs d’essai en abonnés payants, et fidéliser durablement dans un contexte d’abandon précoce ?


**🛠️ Solution apportée (100 % SQL) :**

* Reconstitution complète des parcours clients via fonctions analytiques (`RANK`, `ROW_NUMBER`)
* Création de KPIs : taux de churn, délai avant souscription, taux de conversion par plan
* Segmentation des clients selon leur comportement d’usage
* Identification des profils à risque (essai non actif, churn immédiat)


**📊 Résultats clés :**

* 19,4 % des utilisateurs quittent sans tester de plan payant
* Le **plan annuel** génère la **meilleure rétention**
* Le churn est très élevé chez les utilisateurs inactifs pendant l’essai


**🧩 Compétences mobilisées :**

* SQL  (RANK, ROW\_NUMBER, modélisation temporelle)
* Analyse de churn et de conversion freemium
* Reconstruction de parcours clients
* Création de KPIs (délai de souscription, taux de churn, plan performance)
* Segmentation comportementale
* Lecture business SaaS : rétention, monétisation, LTV
* Recommandations marketing

➡️ *[Voir le projet](https://github.com/sebastiencaestecker/Optimiser-l-onboarding-client-pour-maximiser-les-conversions-dans-une-offre-freemium)*

---

### 📌 [Analyser la performance d’un réseau de coffee shops – Secteur : Retail](https://github.com/sebastiencaestecker/Booster-la-performance-d-un-coffee-shops-avec-l-analyse-comportementale-client/blob/main/README.md)  

**🎯 Objectif :**
Améliorer la rentabilité, l’efficacité produit et la satisfaction client dans un réseau de coffee shops multi-sites, en analysant les ventes, l’affluence et les comportements d’achat.


**🧠 Problème métier :**

Comment optimiser la gestion commerciale et opérationnelle d’un coffee shop avec plusieurs points de vente ?


**🛠️ Solution apportée (Power BI + DAX + Power Query) :**

* Analyse des ventes par jour, heure, catégorie produit et point de vente
* Cartographie des pics d’affluence vs pics de chiffre d’affaires
* Comparaison des performances par magasin (Hell’s Kitchen, Astoria, Manhattan)
* Identification des produits moteurs du CA (ex : Barista Espresso, Chai Tea)
* Recommandations concrètes sur l’organisation, l’offre produit et les leviers d’optimisation


**📊 Résultats clés :**

* CA mensuel : 166 000 € (+6,2 % vs mois précédent)
* 73 % des ventes concentrées sur la semaine
* Pic d’affluence 8h–11h, surtout le mercredi
* Hell’s Kitchen : +8,3 % de croissance
* Décalage entre affluence et CA ➜ potentiel d’optimisation produit/offre

**📌 Recommandations métier :**

* Optimiser les plannings sur les créneaux critiques (8h–11h)
* Mettre en avant les boissons artisanales premium
* Créer des offres ciblées pour lisser la fréquentation hors-pic
* Piloter chaque point de vente avec un dashboard adapté aux managers
* Valoriser les produits végétaux dans l’offre

**🧩 Compétences mobilisées :**

* Power BI (visualisation, interactivité, navigation UX)
* DAX (SAMEPERIODLASTYEAR, PARALLELPERIOD, DATEADD)
* Power Query (modélisation, transformation de données)
* Analyse produit et performance multi-magasins
* Lecture métier : CA, panier, affluence, segmentation temporelle
* Recommandations orientées retail & satisfaction client
* Construction de dashboard pour les équipes terrain

➡️ *[Voir le projet](https://github.com/sebastiencaestecker/Booster-la-performance-d-un-coffee-shops-avec-l-analyse-comportementale-client/blob/main/README.md)*

---

### 📌 [Optimiser logistique, produit et client pour une pizzeria digitalisée – Secteur : Retail](https://github.com/sebastiencaestecker/Optimiser-l-experience-client-et-la-logistique-dans-la-restauration-rapide/blob/main/README.md)  

**🎯 Objectif :**
Améliorer la rentabilité des menus, l’efficacité des livraisons et la satisfaction client dans un modèle de restauration rapide digitalisée.


**🧠 Problème métier :**

Comment concilier personnalisation des recettes, rapidité de livraison, et rentabilité dans une chaîne de pizzas en ligne ?


**🛠️ Solution apportée (100 % SQL) :**

* Analyse des commandes, recettes et comportements d’achat
* Évaluation de l’impact des personnalisations sur le temps de livraison
* Étude des performances livreurs (vitesse, réussite, distance parcourue)
* Identification des ingrédients les plus modifiés/exclus
* Recommandations concrètes sur l’optimisation produit et logistique


**📊 Résultats clés :**

* 64 % des pizzas sont personnalisées → complexité accrue
* +30 % de temps de livraison pour les commandes modifiées
* Les pizzas végétariennes sont les plus souvent changées
* Vitesse des livreurs : de 10 à 20 km/h selon profil
* Taux de livraison réussie : 87 %


**📌 Recommandations métier :**

* Réduire la carte aux recettes les plus commandées et stables
* Créer des **combinaisons prédéfinies** pour limiter la surcharge de personnalisation
* Former ou repositionner les livreurs les plus lents
* Optimiser les achats selon les exclusions fréquentes
* Mettre en place un **bonus logistique basé sur la performance**

**🧩 Compétences mobilisées :**

* SQL  (jointures, `STRING_AGG`, `STRING_SPLIT`, `CASE`, `CAST`)
* Modélisation temporelle (commande vs livraison)
* Analyse logistique (temps, distance, taux de réussite)
* Lecture business : rentabilité, complexité opérationnelle
* Analyse produit : préférences, exclusions, personnalisation
* Formulation de recommandations opérationnelles concrètes


➡️ *[Voir le projet](https://github.com/sebastiencaestecker/Optimiser-l-experience-client-et-la-logistique-dans-la-restauration-rapide/blob/main/README.md)*

---

### 📌 [Comprendre l’attrition des employés – Secteur : RH ](https://github.com/sebastiencaestecker/Optimiser-la-retention-des-talents-grace-la-data/blob/main/README.md)  

**🎯 Objectif :**
Aider une entreprise tech à **identifier les profils à risque de départ** et à piloter une stratégie de rétention efficace dans un contexte de tension RH.


**🧠 Problème métier :**

Quels sont les facteurs qui précèdent un départ volontaire, et comment les RH peuvent-ils agir avant qu’il ne soit trop tard ?


**🛠️ Solution apportée (Power BI + DAX + Power Query) :**

* Analyse croisée des données RH : ancienneté, poste, satisfaction, déplacements, salaires
* Modélisation d’un tableau de bord RH interactif avec 4 pages clés : Overview, Démographie, Performance, Attrition
* Identification des **profils à risque** (Data Scientists, RH, Sales Reps)
* Intégration de la dimension **diversité & inclusion** (genre, âge, ethnie vs rémunération)
* Recommandations concrètes pour réduire l’attrition et mieux cibler les actions RH


**📊 Résultats clés :**

* Taux d’attrition global : 16,1 %
* Profils les plus exposés : faible ancienneté, surcharge de travail, voyages fréquents
* Départs plus fréquents chez les collaborateurs < 2 ans
* Mise en évidence de **disparités salariales** selon genre et ethnie


**📌 Recommandations métier :**

* Prioriser les actions de rétention sur les jeunes talents
* Réduire les déplacements pour les profils à risque
* Détecter les baisses de satisfaction avant qu’elles n’impactent la fidélité
* Surveiller les écarts salariaux dans une logique d’équité


**🧩 Compétences mobilisées :**

* Power BI (dashboard interactif multi-pages)
* DAX (mesures personnalisées, filtres dynamiques)
* Power Query (nettoyage, transformation, jointures)
* Analyse RH (satisfaction, performance, inclusion)
* Lecture croisée de données démographiques, salariales et comportementales
* Construction d’outils d’aide à la décision RH


➡️ *[Voir le projet](https://github.com/sebastiencaestecker/Optimiser-la-retention-des-talents-grace-la-data/blob/main/README.md)*

---

### 📌 [Définir un loyer juste pour les logements publics – Secteur : Collectivité ](https://github.com/sebastiencaestecker/un-loyer-juste-pour-les-logements-publics)  

**🎯 Objectif :**
Aider une collectivité à fixer un **loyer équitable** pour des logements publics attribués aux agents municipaux, en tenant compte des **réalités socio-économiques locales**.

**🧠 Problème métier :**

Comment fixer un loyer cohérent avec les revenus des agents, les prix du marché, et les conditions de vie territoriales, sans créer d’inégalités ni surpayer le parc ?


**🛠️ Solution apportée (stack 100 % cloud – GCP, SQL, Python, Power BI) :**

* Croisement de données publiques : loyers, revenus fiscaux, sécurité, population, infrastructures
* Modèle de régression linéaire pour prédire un loyer €/m² selon les caractéristiques de la zone
* Création d’un **dashboard Power BI interactif** avec carte des loyers par commune
* Recommandations claires pour une **politique locative juste et transparente**


**📊 Résultats clés :**

* Modèle prédictif fiable basé sur des variables sociales et territoriales
* Identification de zones à **loyer modéré justifié** (présence de services publics, insécurité, revenus faibles)
* Aide à la **grille de loyers différenciée par zone**, au lieu d’un prix fixe arbitraire
* Support de négociation ou de révision future basé sur des **indicateurs objectifs**

**📌 Recommandations métier :**

* Indexer le loyer sur le **revenu médian local**, pas uniquement le marché
* Valoriser les logements bien desservis (transports, services)
* Créer un **barème évolutif** selon les indicateurs socio-territoriaux
* Utiliser la modélisation pour justifier et documenter les décisions RH/immobilières

**🧩 Compétences mobilisées :**

* Python (pandas, sklearn – nettoyage, régression)
* SQL (jointures, préparation sur GCP BigQuery)
* Modélisation prédictive (régression linéaire)
* Power BI (cartographie, filtres dynamiques, simulation visuelle)
* Analyse territoriale (loyer, revenu, sécurité, accessibilité)
* Lecture politique publique et équité sociale via la data
* Orchestration de projet data sur une stack cloud complète (GCP)

➡️ *[Voir le projet](https://github.com/sebastiencaestecker/un-loyer-juste-pour-les-logements-publics)*

---

## 🏆 **Certifications et Formations**

- [**Certification Google Analytics**](https://skillshop.credential.net/1e53a185-38cf-4348-8178-23347463a3d9#acc.xNRIvWQY).
- [**Formation en Data Analyst Fullstack**](https://www.credential.net/9fd25ed9-3b2e-4502-8cac-2b6fcbe4e494#acc.4LUoVDe2)


## 🤝 **Contact**

Je suis toujours à la recherche de nouvelles opportunités pour appliquer mes compétences en analyse de données. 
- **Email** : [sebastien.caestecker@gmail.com](mailto:sebastien.caestecker@gmail.com)
- **LinkedIn** : [Sébastien Caestecker](https://www.linkedin.com/in/sebastien-caestecker-753811139/)

---

