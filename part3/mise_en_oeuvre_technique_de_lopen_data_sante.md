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

Cette partie tente d’évaluer quelles sont les offres de services open data qui pourraient être proposées par ce système national. [...]
