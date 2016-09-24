# 3.2. Mise en œuvre technique de l'open data santé

## 3.2.1. Création du SNDS

Dans un premier temps évoqué dans la Convention d’Objectifs et de Gestion (COG), la création d’un système national des données de santé est confirmée dans les textes du Projet de Loi de Modernisation de notre Système de Santé (PLMSS) :

> « Parce que les enjeux de santé sont en constante évolution, le projet de loi organise un système national des données de santé. Il permettra l’ouverture (open data) des données publiques et un accès compatible avec le secret des données personnelles pour des recherches, projets d’étude et d’évaluation d’intérêt public. ».

À ce jour, la constitution d’un tel système n’est contrainte par aucune technologie. Les particularités majeures que j’identifie sont :- la taille exceptionnelle des bases et- l’obligation de mettre en œuvre les moyens d’une sécurité perfectionnée.Pour rendre le SNDS attractif, il parait judicieux d’intégrer des fonctionnalités selon les concepts relevant de l’agilité pour permettre des évolutions itératives et incrémentales sur le système, et d’y assurer les habilitations contrôlées prévues.

## 3.2.2. Anticipation du fonctionnement du SNDS

Comme précédemment évoqué, le Système National des Données de Santé (SNDS) n’en est qu’au stade de projet : aucune information d’ordre technique n’a été publiée à ce jour. Suite à ce constat, j’ai donc pris l’initiative de rédiger une interview à l’attention de responsables du domaine décisionnel au sein de l’AM (consulter l’annexe 4). Cependant, ce projet n’a pas pu se concrétiser pour des raisons de renouvellement de marché (entre la CNAMTS et Sopra Steria) et de disponibilité des interlocuteurs.

#### Un socle de technologies avancées

Pour appréhender le défi que représente la création d’un tel système, nous partagerons dans cette partie les deux éléments techniques identifiés comme pouvant *a priori* être retenus pour déployer un système aussi particulier.

Concernant les **technologies de stockage**, Oracle est un partenaire clé de l’AM. Il est le principal fournisseur de solutions permettant de supporter la puissance requise par les gigantesques bases, comme le SNIIRAM notamment. Dans cette mesure, la technologie Exadata d’Oracle devrait permettre un interfaçage aisé avec les autres bases déjà en place.

Le SNDS étant distinct des bases originales, un **moniteur de transfert** de fichier serait nécessaire. L’office d’un tel outil est de sécuriser les interactions à base de fichier (volumineux dans le cas présent), qu’il s’agisse d’émission ou de réception. Ce type d’outil a l’avantage de fournir une traçabilité précise des transferts et des comportements constatés (reprises, arrêts). La solution Axway CFT leader sur le marché de la gouvernance de flux pourrait sûrement convenir à cette réalisation.

## 3.2.3. Anticipation sur l'exposition des données du SNDS

Cette partie tente d’évaluer quelles sont les offres de services open data qui pourraient être proposées par ce système national. 

### a. Comparatif

Dans ce paragraphe sont comparés :- d’une part, le téléchargement de fichiers statiques hébergés sur un serveur,- d’autre part, la mise à disposition d’API (sous forme de web services).

|       |     FICHIER STATIQUE    |   API | + |
| :-------------: |: ------------- | :--------- | :----: |
|**Utilisabilité** | Le poids de certaines bases peut-être un frein à l’exploitation. Exemple: DAMIR en ligne est disponible à condition d’en télécharger les 70 fichiers CSV de 500Mo chacun. | Le réutilisateur et/ou l’utilisateur final peut élaborer ses propres jeux de données. Il ne supporte pas le poids des données non pertinentes. | API |
| **Disponibilité des données**      |        Si indisponibilité, la précision est le code de l’erreur HTTP.        |      Si indisponibilité, il y a possibilité de monitorer précisément. Une plateforme de suivi des services pourrait informer de l’état en temps réel des services. | API |
| **Format des données**        |        Non normé et difficilement exploitable dans certains cas. Tableur (CSV, XLS, ODS...), Texte (TXT, DOC...), Autres (PDF, XML...)        |   Simple et normé : XML, JSON | API |
| **Fraicheur des données** |  Difficile à mettre à jour, beaucoup de données deviennent indisponibles.       |      Le temps « réel » est possible. | API |
|**Disponibilité de la plateforme**| Le téléchargement de données sous cette forme, même volumineuses, ne provoque pas d’instabilités graves. | Conséquence de la fraicheur des données. Si la plateforme est mal dimensionnée, que la consultation des Web Services (WS) est trop importante, alors cette plateforme peut être indisponible. | API (~) |
|**Gestion des accès**| Pour un jeu de données, soit l’accès est permis soit il ne l’est pas. |Très paramétrable, via les requêtes.| API |

En synthèse, une mise à disposition de fichier statique n’est pas rédhibitoire et pourrait même être envisagée en addition à une mise à disposition par API. Cependant, le fichier statique ne favorise pas l’exploitation par des réutilisateurs, **à l’inverse de la mise à disposition par API, qui semble être plus profitable** pour les deux parties :- Confère au fournisseur,	- une maitrise et un suivi des services délivrés en termes de qualité et d’accès,	- la possibilité de proposer une offre évolutive dans le temps.
- Offre au réutilisateur et/ou l’utilisateur,	- la garantie d’accéder à des données de qualité (fraicheur, granularité),	- une exploitation selon les standards du Web.
### b. Avantages d’une exposition par Web Services
Outre les avantages tirés de la comparaison précédente, l’exposition d’API, plus précisément de web services, possède d’autres atouts.
#### Maintenance et qualité de service

- **Échelonner l’ouverture des données**. Étape par étape, domaine par domaine (données des bénéficiaires, des établissements de soins, etc.), accès par accès (chercheurs, professionnels de santé, citoyens). L’intérêt figure en plusieurs lieux.	- Pouvoir proposer une offre de services de qualité, disponible et stable.	- Permet la prise en compte des feedbacks des usagers.
- Connaître et suivre les usages qui en sont faits.	- Mesurer l’attractivité des données, la volumétrie afin de garantir une certaine qualité d’usage	- Mesurer l’intérêt des réutilisateurs pour les jeux de données mis à disposition.#### Exploitation

- Les Web Services (WS) ont fait leurs preuves. De nombreux développeurs les utilisent à travers le web : Graph API de Facebook, API SNCF par la SNCF, entre autres. Ils sont également très utilisés en interne dans les organisations, notamment au sein du SI CNAMTS. Leur **mise en œuvre est donc peu coûteuse et très bien maitrisée**.
- La simple mise à disposition d’une console auprès des réutilisateurs (développeurs) les rend plus autonomes et à favoriser l’accessibilité de la plateforme.