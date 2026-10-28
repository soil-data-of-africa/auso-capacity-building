# Renforcement des capacités AUSO

Cette page rassemble des supports de formation, des guides pratiques, des outils et des normes qui soutiennent le développement des capacités tout au long du flux de travail lié aux informations sur les sols.

Les ressources couvrent les principales étapes du travail avec les données pédologiques : planification et échantillonnage sur le terrain, analyses en laboratoire, archivage des échantillons de sol, organisation et harmonisation des données, modélisation et cartographie des sols, ainsi que diffusion et utilisation des informations sur les sols.

Cette collection s'adresse aux pédologues, au personnel de laboratoire, aux gestionnaires de données, aux spécialistes de la cartographie et aux organisations qui développent ou gèrent des systèmes d'information sur les sols, en particulier en Afrique.

Les ressources sont regroupées par étape du flux de travail afin d'aider les utilisateurs à trouver des documents pertinents pour leurs activités. Dans la mesure du possible, chaque entrée précise les objectifs d'apprentissage, le public cible, les prérequis, la langue, le format et les conditions de licence.

Il s'agit d'une collection collaborative et évolutive. Nous accueillons volontiers toute suggestion concernant de nouvelles ressources, des corrections aux éléments existants, ou des retours sur des sujets qui mériteraient d'être mieux couverts. N'hésitez pas à contribuer via les [GitHub Issues](https://github.com/soil-data-of-africa/auso-capacity-building/issues).

## Évaluation des besoins et planification

Avant de mettre en place une campagne, il est essentiel de comprendre les besoins des utilisateurs, l'inventaire des données existantes et les objectifs de l'échantillonnage.

- Le [cadre SIS (SIS framework)](https://resources.isric.org/sis-framework/) propose une méthodologie pour évaluer les besoins liés à un système d'information sur les sols.

## Travail sur le terrain

Les études de terrain nécessitent une préparation minutieuse afin d'être aussi efficaces que possible.

### Stratégie d'échantillonnage

Toute campagne commence par une analyse approfondie visant à déterminer les meilleurs emplacements pour le prélèvement des échantillons.

- [Brus et al., 2022](https://dickbrus.github.io/SpatialSamplingwithR/) propose des orientations utilisant le langage R.

### Organisation de l'échantillonnage

Un outil de type SDMT (outil de gestion et de conception d'échantillonnage) peut faciliter l'organisation d'une campagne de prélèvement. - [Soils for Africa – Manuel SDMT](https://doi.org/10.3030/862900)

### Travail de terrain et échantillonnage des sols

Il existe diverses approches et directives concernant la réalisation des travaux de terrain :

- [Guide de terrain WRB (Annexe 1)](https://wrb.isric.org/documents.html)
- [Manuel de terrain de l'USDA](https://www.nrcs.usda.gov/sites/default/files/2022-09/field-book.pdf)
- [Guide de terrain LDSF (AfSIS)](https://www.landscapealliance.org/publications/pdf/guide/45871-LDSF-Field-Guide-2025.pdf)
- [Soils 4 Africa – Directives pour le travail de terrain](https://africasis.isric.org/res/files/Soils4Africa_D3.3_Guidance_Fieldwork_v01_FINAL.pdf)

Une [série de vidéos](https://www.youtube.com/@soils4africa373/videos), disponibles en plusieurs langues, a été produite par le projet « Soils for Africa » pour accompagner le travail de terrain et le traitement des échantillons.

### Classification des sols

Lors des travaux de terrain, les sols sont généralement classés selon des systèmes de classification locaux et/ou mondiaux :

- [Classification WRB](https://wrb.isric.org/documents.html)
- [Classification selon la taxonomie de l'USDA](https://www.nrcs.usda.gov/sites/default/files/2022-06/Soil%20Taxonomy.pdf)

## Laboratoire

Préparation des échantillons, méthodes analytiques, assurance/contrôle qualité (QA/QC) et gestion des données de laboratoire.

### Préparation et expédition des échantillons

Une préparation et une expédition minutieuses des échantillons permettent d'éviter toute perte de qualité. - [Préparation et expédition des échantillons](https://doi.org/10.3030/862900)

### Analyses en laboratoire

- [Guide pour les analyses en laboratoire](https://africasis.isric.org/res/files/Soils4Africa_D3.4_Guidance_Laboratory_Analysis_v01.pdf)
- [FAO GLOSOLAN – Procédures opérationnelles normalisées (SOP)](https://www.fao.org/global-soil-partnership/Scientific-and-technical-support/networks/the-glosolan/standard-operating-procedures-(sops)/en)

### Assurance et contrôle de la qualité (QA/QC)

- [Assurance et contrôle de la qualité (QA/QC)](https://www.fao.org/global-soil-partnership/Scientific-and-technical-support/networks/the-glosolan/qa-qc/en?utm_source=chatgpt.com)

## Archivage des échantillons de sol

Stockage physique des échantillons, identifiants, inventaires et conservation à long terme.

## Traitement des données

Cette section décrit les différentes étapes du traitement des données.

### Nettoyage et archivage des données

Pendant et après une campagne, les données provenant du terrain et du laboratoire (analyses chimiques, propriétés physiques, spectroscopie proche infrarouge/NIR) doivent être correctement associées et archivées.
Il est préférable d'archiver les données en respectant les principes FAIR dans des dépôts pérennes, en attribuant un identifiant persistant (PID, tel qu'un DOI ou un « Handle ») à chaque jeu de données, afin de faciliter leur référencement dans les publications scientifiques.

- [Soilwise – Stratégie FAIR pour les données et connaissances sur les sols](https://soilwise-he.github.io/soilwise-fair-strategy/)

### Harmonisation des données d'observation

Pour regrouper des données provenant de sources variées au sein d'un jeu de données unique, il est essentiel d'harmoniser les formats, ainsi que les données relatives aux différentes propriétés observées, aux unités de mesure et aux méthodes d'analyse. Par exemple, une valeur de pH mesurée dans une suspension avec un rapport 1:2,5 n'est généralement pas identique à celle obtenue dans une suspension avec un rapport 1:10. Il existe des fonctions de conversion (dites « fonctions de transfert ») permettant de passer d'une méthode à une autre.

- [ISO 28258 – Modèle de données sur les sols et sa mise en œuvre](https://github.com/ISRICWorldSoil/iso-28258) : L'ISRIC gère un modèle de base de données PostgreSQL, conforme à la norme ISO 28258, conçu pour enregistrer des données d'observation sur les sols accompagnées de leurs métadonnées complètes.
- [Soilwise – Encodage des données d'observation sur les sols](https://soilwise-he.github.io/soil-observation-data-encodings/)
- [Soilharmony – Fonctions de transfert](https://github.com/soilharmony) : Ce projet, actuellement en phase de démarrage, devrait offrir un aperçu complet des connaissances existantes sur les fonctions de transfert.
- [ISRIC – Développement de produits d'information sur les sols, harmonisés à l'échelle mondiale et continentale](https://isric.org/focus-areas/soil-information-products/)

### Modélisation et cartographie des sols

Dans de nombreux cas, les cartes des sols sont élaborées par des experts du domaine, qui identifient des zones géographiques présentant des caractéristiques distinctives — souvent récurrentes — en matière de relief, de lithologie, de morphologie de surface, de pente, de matériau parental et de type de sol. Par ailleurs, la cartographie numérique des sols (*Digital Soil Mapping*) repose sur une approche technologique permettant de prédire la répartition des propriétés des sols dans l'espace et dans le temps, en utilisant des données d'observation existantes ainsi que des covariables, telles que le modèle numérique d'élévation, l'indice de surface foliaire, la géologie ou encore l'hydrologie. - [Bases de données numériques mondiales et nationales sur les sols et les terrains (SOTER)](https://files.isric.org/public/documents/isric_report_2013_04.pdf)
- [Préparation des données pour la cartographie numérique des sols (DSM)](https://resources.isric.org/tutorial/dsm_data_preparation/)
- [Géostatistique pour la cartographie des sols](doi.org/10.17027/isric-fdtz-ma12)
- [Apprentissage automatique pour la cartographie numérique des sols](doi.org/10.17027/isric-krcc-9045)

## Utilisation des données pour l'aide à la décision

Les cartes des sols peuvent servir d'outil d'aide à la décision. Pour une réutilisation optimale, mettez vos cartes à la disposition de différentes communautés.

- [Stylisation et analyse de données matricielles (raster) – Bases (QGIS 3)](https://www.qgistutorials.com/en/docs/3/raster_styling_and_analysis.html)
- [Tutoriel sur l'utilisation de SoilGrids avec Python](https://git.wur.nl/isric/soilgrids/soilgrids.notebooks)
- [Utilisation des fichiers « Cloud Optimized GeoTiff » (COG) dans OpenLayers](https://github.com/openlayers/workshop/blob/main/doc/en/cog/README.md)
- [Introduction aux données matricielles (rasters) avec le package « terra » (R)](https://emlab-ucsb.github.io/intro-terra/)
