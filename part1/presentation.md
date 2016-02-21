# 1.1. Présentation

La donnée de santé telle qu’on la connait aujourd’hui est relativement récente. Ces trente dernières années ont vu de nombreux changements se produire. Il n’est plus question de transmettre sa radio ou son carnet de santé de médecins en médecins, l’information médicale est mouvante. L’évolution semble tellement rapide qu’aucune définition légale n’existe en France à son sujet.

Chaque citoyen n’a d’ailleurs pas conscience de l’ensemble des informations qui sont conservées par
l’administration, que celles-ci soient liées à lui, aux soins qu’il consomme, ou encore aux appareils qu’il
utilise. En cela, les données de santé se distinguent en deux parties :

* Une partie des données de santé connues de tous, correspondant aux informations personnelles de l’individu (tailles, poids, antécédents familiaux...).
* Une autre partie, plus discrète mais pourtant bien plus vaste, traitant des informations personnelles mais aussi des dépenses en santé, des honoraires de médecins, des diagnostics, des résultats d’examens ou d’utilisation d’appareils...

À l’image des données globales, dont le volume double tous les deux ans1, les données de santé devraient elles aussi continuer à prospérer. Notamment grâce aux points de collecte toujours plus nombreux et aux coûts de stockage toujours plus faibles.

## 1.1.1. Définition de la donnée de santé

### a. À l'échelle européenne

En mars 2015, la présidence de l’Union Européenne a donné une nouvelle définition, plus complète que la précédente, de la donnée de santé :

> *Les données à caractère personnel concernant la santé devraient comprendre les données se rapportant à l’état de santé d’une personne concernée qui comportent des informations sur la santé physique ou mentale passée, présente ou future de la personne concernée, y compris des informations relatives à l’enregistrement du patient pour la prestation de services de santé, un numéro ou un symbole attribué à un patient, destinés à l’identifier de manière univoque à des fins médicales, des informations obtenues lors d’un contrôle ou de l’examen d’un organe ou d’une substance corporelle, y compris des données génétiques et des échantillons biologiques, ou toute information concernant, par exemple, une maladie, un handicap, un risque de maladie, un dossier médical, un traitement clinique ou l’état physiologique ou biomédical de la personne concernée, indépendamment de sa source, qu’elle provienne par exemple d’un médecin ou d’un autre professionnel de la santé, d’un hôpital, d’un dispositif médical [...].*

Cette définition pointe un périmètre bien plus large qu’auparavant et désormais les informations considérées comme relatives au « bien-être » comme le rythme cardiaque ou l’âge, font figures de données de santé à part entière.

### b. Définition française

La donnée de santé n’a pas de véritable définition légale en France. Cela entraine une confusion entre la donnée de santé à caractère personnel et la donnée de santé à caractère non-personnel.

#### Donnée de santé à caractère personnel
Bien que protégée spécifiquement par le droit au respect de la vie privée ainsi que la loi Informatique et Libertés, celle-ci ne bénéficie pas d’une véritable définition en France. Elle est déterminée par le Groupe de travail Article 29 sur la protection des données (G29 dont fait partie la CNIL) comme étant « *une donnée en relation étroite avec l’état de santé de la personne* ».
Cette donnée se remarque aussi par la possibilité d’identifier une personne via des éléments qui lui sont propres (NIR, date de naissance, dates de soins).

#### Donnée de santé (à caractère non-personnel)
Dans son sens général, désigne les mêmes informations que précédemment mais dans une version
anonymisée, donc a priori sans possibilité de ré-identification directe.
C’est ici que se pose la principale barrière à l’open data santé : le risque de ré-identification ne fait pas consensus. La peur qu’un jour, la progression des technologies couplée à celle des algorithmes permette d’identifier les jeux de données précédemment ouverts

## 1.1.2. Postulat quant aux risques

Avant d’aborder la suite, il est important de préciser la position adoptée pour la poursuite de ce mémoire quant aux données de santé et au respect de la vie privée.

### a. Le risque de ré-identification

Les opposants à l’ouverture évoquent des comportements non-étiques et des mésusages qui pourraient être faits de la part d’employeurs, d’assureurs, etc. À cela peut se poser la question : qui souhaiterait travailler ou être assuré par un organisme cherchant à nuire à un ensemble de personnes ?

Il a toujours été question d’une mise en open data concernant des données « anonymisées ». Mais parler seulement d’anonymisation vis-à-vis des données de l’assurance maladie n’est pas correct, certains jeux de données utilise la pseudonymisation5 (normé ou non).

L’usage de données pseudonymisées – donc conservant un pouvoir d’identification amoindri – devrait n’être réservé qu’aux recherches ou études spécifiques, sous contrainte d’un avis positif de la Commission Nationale Informatique et Libertés (CNIL) et de l’Institut des Données de Santé (IDS).

Aussi, la problématique d’une éventuelle ré-identification apparait surévaluée, toujours dans le cheminement selon lequel les données diffusées en open data seraient à minima pseudonymisées, voire complètement anonymisées, donc sans possibilité de ré-identification directe. En témoigne la conclusion de la dernière mission de la Direction de la Recherche, des études, de l’évaluation et des statistiques (DREES), où celle-ci indique qu’ « *il n’y a pas à l’heure actuelle de mesure du risque de ré- identification et de niveau de risque qui fasse largement consensus dans la communauté des chercheurs ou des producteurs de données* ».
En résumé, une précaution est de mise. Celle-ci devra veiller à ne pas être disproportionnelle et empêcher l’avancement de sujets connexes à ces données de santé.

### b. Le secret médical

La loi est stricte sur la notion de secret médical vis-à-vis des données personnelles, cependant il existe des dérogations au sein du texte fondateur de la Loi informatique et Libertés. À la fois sur le partage mais aussi sur le traitement des données médicales :

« *Nonobstant les règles relatives au secret professionnel, les membres des professions de santé peuvent transmettre les données à caractère personnel qu'ils détiennent dans le cadre d'un traitement de données [...].* ». Loi Informatique et Libertés, article 55.

Il n’est pas question ici de remettre en question cette protection accordée aux données personnelles de santé, mais il s’agit de souligner que certains acteurs peuvent déjà bénéficier d’autorisations pour traiter la donnée médicale personnelle.
