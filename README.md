# Sébastien Caestecker - Data Analyst | Analyse métier | SQL • Power BI • Python • dbt • GCP • Azure


## 👨‍💼 **À Propos de Moi**

Bonjour ! Je suis Sébastien Caestecker, un Data Analyst de 32 ans, passionné par l'ensemble des domaines de la data. Fort de 10 années d'expérience dans le secteur de la grande distribution, j'ai eu l'opportunité de travailler sur une variété de projets, couvrant l'analyse des ventes, l'optimisation des processus opérationnels, ainsi que la prédiction des tendances du marché.

---

## 🎯 **Compétences Clés**

| Domaine                   | Outils                                                                                   |
|---------------------------|------------------------------------------------------------------------------------------|
| **Exploration & Analyse** | SQL (PostgreSQL, BigQuery, SQL Server), Python (Pandas, Numpy, Matplotlib), Excel        |
| **Data Viz**              | Power BI, Tableau                                                                        |
| **Cloud**                 | Google Cloud Platform (BigQuery, Cloud Storage, Notebooks) , Azure                       |
| **Prédiction**            | Python (scikit-learn)                                                                    |
| **API & Web Scraping**    | Python (requests, BeautifulSoup, Scrapy)                                                 |
| **Documentation**         | Notion, Markdown, GitHub                                                                 |






## 🌍 [Projets data orientés métier](https://github.com/sebastiencaestecker?tab=repositories)

---

### 📌 [Fidéliser les clients Silver via une campagne ciblée – Secteur : Retail / e-commerce](https://github.com/sebastiencaestecker/Ciblage_campagne_pour_booster_vente_saisonniere)

**🎯 Objectif** :
Renforcer la fidélité et la valeur du segment Silver en activant une catégorie stratégique peu consommée mais très margée : *Outerwear & Coats*.

**🛠️ Stack :** BigQuery SQL

**💡 Ce que j’ai appris :**

* Identifier des opportunités d’activation via une **analyse RFM croisée au comportement produit**
* Utiliser `PERCENTILE_CONT()` pour le scoring RFM et `RAND()` pour créer un **groupe témoin aléatoire (10 %)**
* Simuler un **ROI de campagne CRM réaliste** en tenant compte du panier, de la marge et du taux de conversion estimé
* Estimer le taux de conversion en se basant sur les campagnes précédentes
* Structurer une campagne CRM testable et exploitable par une équipe marketing

**✅ Résultats & recommandations :**

* 1 820 clients Silver ciblés (actifs mais non acheteurs de manteaux)
* Offre proposée : **25 € dès 100 €** → ROI estimé : **x1,97**
* La campagne ciblée (conversion estimée à 5 %) est **3 à 4 fois plus efficace** que la promotion -70 % des soldes (conversion observée : 0,6 %)

**📌 Recommandations métier :**

* Utiliser ce type de logique pour créer des **campagnes ciblées mesurables**
* Croiser le scoring RFM avec les **marges et paniers par catégorie** pour calibrer la générosité
* Ciblage via un pipeline SQL + BIGQUERY

➡️ *[Voir le projet](https://github.com/sebastiencaestecker/Ciblage_campagne_pour_booster_vente_saisonniere)*


---

### 📌 [Segmenter sa base client par RFM – Secteur : Retail / e-commerce](https://github.com/sebastiencaestecker/Segmentation_RFM_SQL)

**🎯 Objectif** : Identifier les segments clients les plus rentables et définir des actions marketing adaptées.

**🛠️ Stack** : BigQuery SQL

**💡 Ce que j’ai appris** :

* Construire une **segmentation RFM** à partir de comportements d’achat.
* Utiliser `PERCENTILE_CONT()` pour un découpage en **quartiles réels** 
* Concevoir une analyse SQL, de l’agrégation brute jusqu’au scoring CRM pour faire des **recommandations pour un responsable marketing**.

**✅ Résultats & recommandations** :

* Les **clients Platine et Gold** représentent **38 % de la base** mais génèrent **près de 48 % du chiffre d’affaires**.
* Le segment **Silver**, majoritaire, est **sous-exploité commercialement**.
* Le segment **Iron** génère très peu de valeur malgré un coût d’acquisition équivalent.

**📌 Recommandations métier** :

* Fidéliser les clients Platine via un **programme VIP ou offres exclusives**.
* Activer le potentiel du segment Silver par des **promotions à seuil ou du cross-sell**.
* Exclure ou réactiver les clients Iron avec des campagnes ciblées à faible coût.

➡️ *[Voir le projet](https://github.com/sebastiencaestecker/Segmentation_RFM_SQL)*


---

### 📌 [Optimiser l’onboarding dans un modèle freemium – Secteur : SaaS / e-commerce](https://github.com/sebastiencaestecker/Optimiser-l-onboarding-client-pour-maximiser-les-conversions-dans-une-offre-freemium)  
**🎯 Objectif** : Comprendre les parcours utilisateurs pour améliorer la conversion des abonnés.  
**🛠️ Stack** : SQL 

**💡 Ce que j’ai appris** :  
- Approfondir la **modélisation temporelle** des parcours utilisateurs.  
- Manipuler des **fonctions analytiques SQL** : `RANK()`, `ROW_NUMBER()` pour créer des séquences comportementales.  
- Penser l’analyse sous l’angle de la **valeur client** et de la **durabilité du modèle économique**.  
- Comprendre les enjeux clés du business : conversion, rétention, lifetime value.
  
**✅ Résultats & recommandations** :  
- **19,4 %** des utilisateurs annulent après l’essai gratuit, sans tester de plan payant.  
- Les clients qui souscrivent un **plan annuel** sont les plus fidèles.  
- Le **churn est plus élevé** chez les utilisateurs peu actifs durant la période d’essai.
**📌 Recommandations métier** :  
- Proposer une **offre promotionnelle ciblée** à la fin de l’essai gratuit.  
- Mettre en place un **email de réassurance** personnalisé avant la fin de l’essai.  
- Détecter les **signaux faibles de churn anticipé** : faible fréquence d’usage, sessions trop courtes, inactivité.  

➡️ *[Voir le projet](https://github.com/sebastiencaestecker/Optimiser-l-onboarding-client-pour-maximiser-les-conversions-dans-une-offre-freemium)*

---

### 📌 [Analyser la performance d’un réseau de coffee shops – Secteur : Retail](https://github.com/sebastiencaestecker/Booster-la-performance-d-un-coffee-shops-avec-l-analyse-comportementale-client/blob/main/README.md)  
**🎯 Objectif** : Améliorer les ventes, la gestion produit et les horaires d’ouverture grâce à l’analyse multi-sites.  
**🛠️ Stack** : Power Query, Power BI, DAX, modélisation temporelle 

**💡 Ce que j’ai appris** :  
- Maîtriser les filtres temporels avancés avec `SAMEPERIODLASTYEAR`, `PARALLELPERIOD`, `DATEADD` pour enrichir les analyses.  
- Travailler la **granularité temporelle** (jour, heure, semaine).  
- Concevoir un **dashboard interactif**  
- Objectifs de rentabilité, de satisfaction client et d’optimisation opérationnelle.
  
**✅ Résultats & observations clés** :  
- CA mensuel : **166K€**, en hausse de **+6,2 %** vs mois précédent.  
- **73 % des ventes** concentrées en semaine (lundi à vendredi).  
- **Heures de forte affluence** : 8h–11h, avec un pic le mercredi matin.  
- Les **produits les plus rentables** : Barista Espresso, Brewed Chai Tea, boissons chaudes personnalisées.  
- Magasin leader : **Hell’s Kitchen**, +8,3 % de croissance.  
- Décorrélation entre affluence et CA → opportunité d’optimisation produit/offre.
**📌 Recommandations métier** :  
- Optimiser les **plannings d’équipe** sur les créneaux 8h–11h, notamment les mercredis et vendredis.  
- Mettre en avant les **boissons artisanales premium**, contributrices clés au CA.  
- Proposer des **offres combo ou happy hours** pour lisser la fréquentation en heures creuses (soirées, week-ends).  
- Piloter **chaque point de vente individuellement**, avec un suivi simplifié adapté aux managers locaux.  
- Valoriser l’offre végétale dans la gamme café pour répondre aux nouvelles attentes clients.

➡️ *[Voir le projet](https://github.com/sebastiencaestecker/Booster-la-performance-d-un-coffee-shops-avec-l-analyse-comportementale-client/blob/main/README.md)*

---

### 📌 [Optimiser logistique, produit et client pour une pizzeria digitalisée – Secteur : Retail](https://github.com/sebastiencaestecker/Optimiser-l-experience-client-et-la-logistique-dans-la-restauration-rapide/blob/main/README.md)  
**🎯 Objectif** : Améliorer la rentabilité via l’analyse des commandes, livraisons, préférences clients.  
**🛠️ Stack** : SQL

**💡 Ce que j’ai appris** :  
- Approfondir la **modélisation temporelle** dans SQL (temps de commande vs livraison).  
- Manipuler des fonctions avancées : `STRING_SPLIT`, `STRING_AGG`, `CASE`, `CAST`.  
- Travailler la **logique métier retail** et formuler des recommandations.   
- Traduire une base de données en **décisions stratégiques** et visuellement compréhensibles.
  
**✅ Résultats & recommandations** :  
- 64 % des pizzas livrées sont **modifiées** → complexité accrue.  
- Les personnalisations augmentent le **temps de livraison de +30 %**.  
- Les **pizzas végétariennes** sont les plus personnalisées.  
- Forte **disparité entre livreurs** : vitesses moyennes de 10 à 20 km/h.  
- **Taux de livraison réussie** global : 87 %.  
**📌 Recommandations métier** :  
- Réduire la carte aux **recettes les plus commandées** avec le moins de modifications.  
- Simplifier la personnalisation via des **combinaisons prédéfinies**.  
- Former les livreurs les plus lents ou les affecter à des **plages horaires creuses**.  
- Optimiser les **achats d’ingrédients** en fonction des exclusions fréquentes.  
- Proposer un **bonus logistique** basé sur la performance (vitesse, distance parcourue, ponctualité).  

➡️ *[Voir le projet](https://github.com/sebastiencaestecker/Optimiser-l-experience-client-et-la-logistique-dans-la-restauration-rapide/blob/main/README.md)*

---

### 📌 [Comprendre l’attrition des employés – Secteur : RH ](https://github.com/sebastiencaestecker/Optimiser-la-retention-des-talents-grace-la-data/blob/main/README.md)  
**🎯 Objectif** : Identifier les facteurs de départ des collaborateurs dans une entreprise tech fictive.  
**🛠️ Stack** : DAX, Power BI, Power Query 

**💡 Ce que j’ai appris** :  
- Approfondir la **modélisation temporelle** et la gestion des jointures dans Power BI.  
- Renforcer mes compétences en **DAX** et **Power Query**.  
- Concevoir un **dashboard orienté métier**, simple, clair pour les RH.
  
**✅ Résultats & recommandations** :  
- Identification de postes à fort turnover : **Sales Reps, RH, Data Scientists**.  
- Mise en évidence de **facteurs aggravants** : heures supplémentaires, voyages fréquents, faible ancienneté.  
- Ciblage des **profils en perte de satisfaction**, avant que la situation ne se dégrade.  
- **Actions de rétention prioritaires** recommandées sur les jeunes talents (< 2 ans d’ancienneté).  
- Sensibilisation à l’impact de **l’équilibre vie pro/perso** et des déplacements fréquents sur la fidélité.

➡️ *[Voir le projet](https://github.com/sebastiencaestecker/Optimiser-la-retention-des-talents-grace-la-data/blob/main/README.md)*

---

### 📌 [Définir un loyer juste pour les logements publics – Secteur : Collectivité ](https://github.com/sebastiencaestecker/un-loyer-juste-pour-les-logements-publics)  
**🎯 Objectif** : Identifier les facteurs qui influencent les loyers pour proposer des tarifs équitables aux agents publics.  
**🛠️ Stack** : SQL, Python, Power BI, Google Cloud Platform 

**💡 Ce que j’ai appris** :  
- Me familiariser avec la **modélisation prédictive** sur des données socio-territoriales.  
- Gérer une **stack cloud complète** (GCP : BigQuery, Cloud Storage, Notebooks).  
- Créer une **carte thématique dynamique** dans Power BI pour visualiser les disparités.
  
**✅ Résultats & recommandations** :  
- Création d’un **référentiel prédictif de loyers**, cohérent avec les caractéristiques locales.  
- Détection de zones où un loyer plus bas pouvait être justifié (ex. forte criminalité, forte présence de services publics).  
- **Recommandations métier** :  
  - Fixer un **loyer ajusté aux revenus moyens** de la zone, sans s’aligner automatiquement sur le marché.  
  - Valoriser les logements bien **desservis** par les transports, même à loyer égal.  
  - Créer une **grille différenciée** par zone et indicateurs socio-économiques.  
  - Utiliser le modèle comme **base de négociation** ou de revalorisation équitable.
    
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

