# 1.2. Une multiplication des gisements de données

La donnée de santé est présente à travers différents supports. Ceux-ci contiennent plus ou moins de données personnelles, sont plus ou moins pertinents selon le traitement que l’on souhaite en faire et sont aussi plus ou moins concernés par l’ouverture des données de santé telle qu’il en est question dans ce mémoire.

## 1.2.1. Le parcours de soin

Lorsqu’un individu tombe malade, il prend rendez-vous avec son médecin qui lui prescrit des « soins ». Cette transaction est enregistrée par l’assurance maladie si le patient utilise une feuille de soin ou bien sa carte vitale.

Ce parcours de soin est générateur de données :

- les diagnostics réalisés par le médecin,
- les actes réalisés par le médecin,
- les soins et médicaments prescrits,
- montant des remboursements,
- durée de l’arrêt de travail,
- etc.

Le parcours de soin est actuellement l’étape qui génère le plus d’informations aussi hétérogènes soient elles.

## 1.2.2. Les référentiels

Beaucoup de données figurent dans les référentiels. Nous y retrouvons l’exhaustivité des établissements de santé, les professionnels de santé (RPPS) ou encore les bénéficiaires (RNIAM) figurent dans les bases de données maintenues par l’Agence des Systèmes d'Information Partagés de santé (ASIP) ou bien la Caisse Nationale d’Assurance Maladie des Travailleurs Salariés (CNAMTS) :

| Référentiel   |                       Intitulé                                            |
| :-----------: | :------------------------------------------------------------------------ |
| RNIAM[^9]     | Répertoire national interrégimes des bénéficiaires de l’assurance maladie |
| RPPS[^10]     | Répertoire Partagé des Professionnels de Santé                            |
| ...           | ...                                                                       |

Ces données peuvent être considérées comme « dynamiques », puisque le rythme d’actualisation des référentiels est régulier.

## 1.2.3. Les objets connectés de santé


L’Internet des objets est l’un des grands sujets en cours actuellement et pour les prochaines années. Pour preuve, le cabinet Deloitte annonce qu’en 2020, plus de 26 milliards d’objets connectés seront utilisés dans le monde. L’étude précise que ces objets seront essentiellement détenus par des organisations.


En 2019, le marché des objets connectés de santé devrait représenter 5,8 milliards d’euros selon une étude du groupe Xerfi[^1].

Les données qui émanent des objets connectés peuvent être qualifiées de « fluide ». Elles donnent lieu à des flux d’échange quasi temps réel et sont sujets à des traitements permanents. Ce gisement constitue assurément l’avenir prochain de la donnée de santé. Par ailleurs, ce type de technologie remporte une franche adhésion auprès des français.[^2]

### a. Les dispositifs médicaux[^3]

Il s’agit là des dispositifs médicaux connectés qui sont mis à disposition par les établissements de santé ou bien sont distribués par l’assurance maladie. Ces objets peuvent être implantés[^4] ou non et ont la particularité d’émettre ou de recevoir des informations via le réseau.

L’un des plus larges exemples en France est l’appareil à ventilation en Pression Positive Continue (PPC) pour lutter contre l’apnée du sommeil. Cet **objet est équipé d’un accès aux réseaux télécoms pour transmettre les données relatives à l’observance** de ce protocole de soin. Si l’observance n’est pas respectée par le bénéficiaire, alors l’assurance maladie stoppe les remboursements inhérents à la location de l’appareil. Toutefois, le Conseil d’État a annulé en décembre 2014 les arrêtés ministériels relatifs à ce mode prise en charge conditionnée[^5].

Comme nous pouvons le voir avec l’exemple cité ci-dessus, ces nouveaux outils techniques et très variés trouvent leurs avantages essentiellement dans l’e-santé, un secteur en forte croissance.

La télémédecine[^6], qui fait partie intégrante de l’e-santé, décuple l’exploitation de ce potentiel en incluant ces objets au cœur des actes du parcours de soin :

- téléconsultation,
- téléexpertise,
- télésurveillance,
- téléassistance,
- réponse médicale.

Nous pouvons donc mesurer l’importance en termes de quantité et de qualité que représente cette source de données.

Enfin, même si ces données ne sont pas détenues à 100% par l’assurance maladie (mais par des opérateurs tiers agréés), il serait souhaitable que ces données puissent être ouvertes afin, pour poursuivre l’exemple précité, d’améliorer le taux d’observance des traitements.

### b. Le quantified self ou la quantification de soi

La quantification de soi est un phénomène récent qui désigne le fait d’enregistrer, de mesurer et de partager des informations personnelles à l’aide d’applications mobile, d’applications web ou bien de capteurs intégrés à des objets de la vie courante[^7].

Les données récoltées sont stockées par l’utilisateur lui-même, ou bien dans le cloud d’entreprises privées. Ces données sont à différentier de celles obtenues dans le cadre des dispositifs médicaux car les données dont nous parlons ici sont obtenues hors d’un contexte médical. Cependant les informations récupérées peuvent être identiques à celles mesurées avec un dispositif médical.


> L’exploitation des données issues de la quantification de soi laisse face à quelques interrogations[^8]. Les données obtenues dans le cadre d’une quantification de soi ont la particularité d’être :

> - non-normées pour la plupart,
- d’une qualité plus ou moins intéressante,
- très nombreuses, voire trop,
- d’une pertinence très variable,
- et hétérogènes.

Les données de quantification de soi détenues par des entreprises privées ne font actuellement pas l’objet d’une demande d’ouverture, compte tenu de la loi CNIL de 1978. Toutefois, comme nous le verrons dans la suite de ce mémoire, des tentatives ont été menées pour rapprocher ces deux types de données (données de santé et données de quantification de soi).

---

[^1] Le marché des objets connectés - Prévisions pour 2016 et perspectives à moyen terme - Paysage concurrentiel et mutations de l'offre, Groupe XERFI, [www.xerfi.com/presentationetude/Le-marche-des-objets-connectes_4EEE16](www.xerfi.com/presentationetude/Le-marche-des-objets-connectes_4EEE16)

[^2] Étude réalisée par TNS Sofres pour le compte de La Mutuelle Générale, « Les Français et les technologies au service de l’autonomie des personnes atteintes de maladies neurodégénératives. », [http://www.tns- sofres.com/sites/default/files/maladiesneurodegeneratives.pdf](http://www.tns- sofres.com/sites/default/files/maladiesneurodegeneratives.pdf)

[^3] L’article L.5211-1 du code de la santé publique définit ce qu’est un dispositif médical du point de vue de la législation.

[^4] Dispositifs Médicaux Implantés (DMI)

[^5] Apnée du sommeil et dispositif médical à PPC : annulation du conditionnement du remboursement à l'observance,
[www.vidal.fr/actualites/14547/apnee_du_sommeil_et_dispositif_medical_a_ppc_annulation_du_conditionnement_du_rembou rsement_a_l_observance/](www.vidal.fr/actualites/14547/apnee_du_sommeil_et_dispositif_medical_a_ppc_annulation_du_conditionnement_du_rembou rsement_a_l_observance/)

[^6] Fiches pédagogiques d’aide à la qualification d’un projet de télémédecine (01/2015), [http://esante.gouv.fr/sites/default/files/asset/document/asip_fiches_telemedecine_bd.pdf](http://esante.gouv.fr/sites/default/files/asset/document/asip_fiches_telemedecine_bd.pdf)

[^7] Ces capteurs peuvent être sous forme de montres, ceintures, lentilles de contact, balances, fourchettes, etc.

[^8] Le quantified self est suivi de près par la CNIL, Cf : Cahier IP 2, Bibliographie, [https://www.cnil.fr/sites/default/files/typo/document/CNIL_CAHIERS_IP2_WEB.pdf](https://www.cnil.fr/sites/default/files/typo/document/CNIL_CAHIERS_IP2_WEB.pdf)

[^9] Le [RNIAM](https://www.cnil.fr/fr/rniam-repertoire-national-interregimes-des-beneficiaires-de-lassurance-maladie-0)

[^10] Les données du [RPPS](http://esante.gouv.fr/services/referentiels/identification/acceder-aux-donnees-du-rpps-0)