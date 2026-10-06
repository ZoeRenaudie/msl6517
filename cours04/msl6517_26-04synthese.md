# Les interfaces publiques et les catalogues en ligne des musées

**MSL6517 Inventaire et traitement des données, séance 4 (asynchrone)** Synthèse du cours en ligne. 

Zoë Renaudie, Université de Montréal

Les systèmes d'information des musées disposent de plus en plus d'interfaces publiques qui donnent à voir la collection. La conception d'un catalogue en ligne n'est pas neutre : elle engage des choix de structuration des données, de médiation et de rapport au visiteur. Cette séance les examine à travers la notion de *generous interfaces* et la question du discours que le musée construit en ligne sur sa collection.

La **documentarisation généralisée** (« documentalité » chez Ferraris, « hyperdocumentarisation ») désigne la transformation de nos interactions et de notre environnement en données et en documents. Le catalogue des collections en est un exemple emblématique : pièce maîtresse de la médiation institutionnelle, il met aussi en jeu de nouvelles compétences documentaires.

## 1. Pourquoi des catalogues en ligne ?

### 1.1 Le constat de Simard (2001)

Pour Françoise Simard, les bases de données d'inventaire sont d'intérêt public mais « muettes » pour le grand public : naviguer dans une base d'inventaire revient à visiter des réserves sans signalisation, sans ordre logique, sans mise en contexte ni éclairage. Leurs informations textuelles et iconographiques sont riches, mais non scénarisées. Le problème est donc d'abord un problème de **navigation**.

**Questions** : depuis 2001, les interfaces ont beaucoup évolué; d'après votre usage, sont-elles efficaces ? Pourquoi les catalogues en ligne sont-ils bien plus que de simples bases de données ?

### 1.2 Objectifs du catalogue

Les objectifs reprennent, transposés des livres aux œuvres, ceux de Charles A. Cutter (*Rules for a Printed Dictionary Catalogue*, 1876) :

- **trouver** une œuvre (par auteur, titre, sujet s'il est connu);
- **rassembler** : présenter les ressources de la collection (par auteur, sujet, domaine);
- **choisir** : assister le choix des œuvres (par édition, genre).

Les tâches utilisateur de l'IFLA LRM ajoutent *identifier*, *obtenir* et surtout **explorer**. Ce dernier verbe distingue le plus les catalogues muséaux actuels (interfaces généreuses, parcours, récits). *Question* : voyez-vous d'autres objectifs ?

### 1.3 Lien avec la base de gestion

Le catalogue public est souvent alimenté par la base de gestion des collections. 

Modes de liaison habituels :

![schema-base-gestion-catalogue(1)](../imagesMSL/schema-base-gestion-catalogue(1).png)

## 2. Repères chronologiques

### 2.1 Musées et bibliothèques

Les bibliothèques ont très tôt développé des systèmes d'information partagés. Le phénomène est plus tardif dans les musées, pour trois raisons :

- la diversité des collections (ethnographiques, scientifiques, artistiques) implique des domaines de connaissance et des modèles métiers variés;
- les bibliothèques pouvaient économiser en partageant leurs notices, alors que les musées gèrent surtout des *unica* et avaient moins d'incitation à partager;
- les musées ne se sont fortement engagés dans la numérisation que ces dernières années, avec un grand impact sur leurs approches documentaires.

### 2.2 Les OPAC

Un *Online Public Access Catalog* est un catalogue, principalement de bibliothèque, accessible en ligne. Il a été rendu possible par le format MARC (finalisé en 1968) et a remplacé les fichiers papier. Les premiers grands catalogues en ligne datent de l'Ohio State University (1975) et de la Dallas Public Library (1978), avec des interfaces textuelles. Depuis la fin des années 1990, l'interface est le plus souvent graphique. L'OPAC est généralement fourni par le système intégré de gestion de bibliothèque (SIGB).

Côté musées : création du CIDOC (1963), Museum Computer Network (1967), Information Retrieval Group of the Museums Association, IRGMA (1967-1977). Pour aller plus loin : Parry 2007, Borgman 1996.

### 2.3 Six décennies d'informatique muséale

- **1970, premiers développements.** Pression pour démontrer l'*accountability* envers les collections, création de services d'audit, premiers systèmes informatiques dans les universités et collectivités. Au Royaume-Uni, la Museum Documentation Association (MDA, 1977) produit standards, manuels, systèmes de catalogage sur fiches et le logiciel MODES. Priorité à l'inventaire, au contrôle et à la responsabilité; arrivée de premiers spécialistes de l'information.
- **1980, micro-informatique.** Généralisation, systèmes « maison », spécialisation croissante des rôles. Première conférence sur la gestion des collections dans les musées (1987).
- **1990, société de l'information et standardisation.** SPECTRUM, travaux sur la terminologie, projet CIMI, initiatives européennes (EMII), convergence entre musées, bibliothèques et archives (GLAM). Les plus grands musées se dotent de départements de documentation. Adoption très large de SPECTRUM au Royaume-Uni.
- **2000, numérisation de masse et diffusion web.** Politiques gouvernementales tournées vers l'accès, attentes croissantes du public. On passe d'une focalisation sur l'inventaire à une focalisation sur l'information, avec des systèmes actifs tournés vers l'accès et des collaborations avec le monde académique.
- **2010, ouverture et participation.** Les musées adoptent des politiques d'Open Access et d'Open Data : Rijksstudio (2012-2013, 125 000 images, puis près de 200 000), programme Open Access du Met (2017, 375 000 images en CC0), Louvre (480 000 notices, réserves comprises). Les visiteurs participent à l'enrichissement des données (étiquetage, transcription, annotation : Zooniverse, Wikimedia Commons, *Tag! You're It* du Brooklyn Museum). Enjeux : licences des reproductions numériques, biais coloniaux des catalogues (*Words Matter*), restitutions numériques (Benin Dialogue Group).
- **2020, IA, personnalisation et pérennité.** La personnalisation adapte les parcours au comportement de l'utilisateur, avec gamification et communautés en ligne. L'IA entre dans les catalogues. 

### 2.4 Les musées en ligne

- **1992** : en France, la base Joconde sur Minitel (3614 Joconde), avec plus de 120 000 descriptions de peintures, dessins et gravures dans plus de 60 musées.
- **Fin 1994** : une vingtaine de musées ont un site web; plus de 70 en février 1995, plus de 130 en mai, plus de 200 début 1996. 1996 est un point de bascule : tous les musées nationaux canadiens et la plupart des musées provinciaux sont en ligne.
- **1994** : le musée des Arts et Métiers investit le web; exposition *Le Siècle des Lumières dans les musées de France* (ministère de la Culture, INRIA), avec une dimension pédagogique et l'idée de musée virtuel.
- **2004-2008** : émergence du web social.

Ces débuts se font souvent sans personnel qualifié, avec le recours fréquent à des prestataires et à des logiciels open source pour garantir la continuité. Soutiens institutionnels : Direction des musées de France, RMN, plan gouvernemental de 1998 pour la société de l'information.

**Le cas du Louvre** : il permet de suivre trente ans d'évolution, de la vitrine au service (billetterie, boutique), puis au catalogue exhaustif.

| Année | Événement |
| --- | --- |
| 1994 | CD-ROM; le site indépendant Web-Louvre pousse le musée à réagir |
| 1995 | Ouverture du site (juillet) |
| 1996 | Louvre.fr et réservations en ligne |
| 1999 | Cyberboutique |
| 2000 | Près de 6 millions de visites en ligne, autant que de visiteurs réels |
| 2001 | Crise de croissance, seconde version soutenue par le mécénat (projet Cim@ise) |
| 2010 | Partenariat avec Orange, « communauté Louvre » (fermée en octobre 2011) |
| 2021 | collections.louvre.fr (plus de 480 000 notices) et refonte *mobile-first* |
| 2026 | Refonte des outils de gestion des collections en cours |

## 3. Chercher dans un catalogue

**Recherche simple.** Recherche sur tous les termes, comme un moteur de recherche.

**Recherche multicritère (experte).** Elle suppose de connaître les structures internes du système (champs, termes d'indexation, opérateurs). Les efforts récents portent sur les opérateurs booléens (ET, OU, SAUF), le multicritère et l'auto-complétion. Ressource à consulter : le [guide des opérateurs de recherche](https://bibliotheque.uqac.ca/sofia/guide/operateurs-de-recherche) de la bibliothèque de l'UQAC.

**Recherche à facettes.** L'utilisateur explore une collection en lui appliquant des filtres. Elle répond à la rigidité des systèmes de représentation et au chaos des index non structurés. Trois paradigmes se sont succédé depuis le web :

- la navigation hiérarchique de type taxonomique (par exemple DMOZ, jusqu'en 2017);
- la recherche directe par mots, popularisée par les moteurs;
- la recherche à facettes, qui combine les deux : on navigue dans un espace multidimensionnel en restreignant chaque dimension.

Une classification à facettes organise chaque élément selon des dimensions explicites (les facettes), correspondant habituellement à ses propriétés, parcourues dans l'ordre voulu. S. R. Ranganathan (1892-1972) en est le précurseur, avec les *Cinq lois de la science des bibliothèques* (1931) et la Colon Classification (1933), fondée sur cinq facettes (Personality, Matter, Energy, Space, Time). Pour l'utilisateur, la navigation par facettes élimine les impasses (*dead ends*) dues à des combinaisons de contraintes inadéquates (Tunkelang 2009).

**Approche classificatoire.** De nombreux catalogues privilégient les entrées par techniques (souvent calquées sur l'organisation du musée), chronologie, écoles et courants; pour l'art moderne et contemporain, la périodisation en décennies remplace les coupes historiques usuelles (filtres du MoMA). Pour Corinne Welger-Barboza, ces catégories, installées par la mise en ordre du patrimoine (Recht 1998), sont la marque du point de vue historiographique du musée.

**Recherche sémantique.** Moteurs en langage naturel, agents conversationnels (Anna à Reims). Même avec l'IA, la maîtrise de la logique booléenne, des guillemets et de la troncature reste la compétence clé des professionnels de l'information pour fouiller de vastes bases sans perte de pertinence. *Question* : qu'est-ce qui change dans la recherche aujourd'hui avec les chatbots ?

## 4. Regarder un catalogue

Grille de lecture :  
- quels sont les points d'accès ? 
- Comment navigue-t-on dans les ressources ? 
- Comment les visualise-t-on ? Peut-on les manipuler (tagger, stocker) ? 
- Quel discours sur la collection le catalogue construit-il ?

### Études de cas

- **[Tate Online](http://www.tate.org.uk).** Site lancé en 1998 et relancé en 2000 pour Tate Modern; d'abord pensé comme une cinquième galerie, puis intégré transversalement aux activités (stratégie 2010-2012 de John Stack). Descripteurs en grande partie tirés d'Iconclass; trois types de données (cartel, *highlights*, descripteurs). Le même thésaurus sert à décrire les œuvres et à naviguer. L'interface est paradoxale, mêlant mots-outils et description savante.
- **[Victoria & Albert Museum](http://collections.vam.ac.uk/).** Plusieurs entrées (suggestions des œuvres les plus recherchées, interface plus complète).
- **[SFMOMA](https://www.sfmoma.org).** [Artscope (Stamen)](https://stamen.com/work/sfmoma-artscope/) est un catalogue comme espace d'expérimentation; aujourd'hui, retour à des interfaces classiques et similaires d'un musée à l'autre, sans interopérabilité accrue des données.
- **[Rijksstudio](https://www.rijksmuseum.nl/en/rijksstudio).** Rijksmuseum rouvert en avril 2013 après dix ans de rénovation; site présenté le 30 octobre 2012. « L'image est l'interface » (Peter Gorgels). 125 000 œuvres libres de droits au lancement; partage, modification, téléchargement. Seules 8 000 œuvres sur 1 100 000 sont exposées. Bilan de Martijn Pronk (2015) : environ 15 millions de visites, 200 000 comptes, près de 500 000 collections personnelles, plus de 1,3 million d'images téléchargées. Images déposées sur Wikimedia Commons; conception en mode « app », *responsive*.
- **[National Galleries Scotland](https://www.nationalgalleries.org/art-and-artists) (2017).** Sur l'ancien site, 6 % des quelque 90 000 objets étaient disponibles; la totalité l'est désormais (février 2018). Développement agile, open source (Drupal, Apache Solr, Amazon S3), extraction de couleurs, approche mobile.
- **[Barnes Collection Online](https://collection.barnesfoundation.org) (2017).** Catalogue financé par la Knight Foundation, code en open source (extraction depuis TMS). Il prolonge le parti pris d'Albert Barnes (ensembles formels de lumière, d'espace, de couleur et de ligne) : vision computationnelle, regroupement par similarité visuelle (*Visually Related*).
- **[Sarjeant Gallery](https://collection.sarjeant.org.nz) (2017).** Google Vision API; site explorable sans connaissance préalable de la collection; conformité WCAG 2.0 AA; phrases en langage naturel inspirées du Cooper Hewitt; filtres par couleur.
- **[LACMA](https://seasian.catalog.lacma.org/).** Catalogue en ligne interactif avec espace de visualisation (zoom, combinaison de vues) pour l'examen comparatif; publiable aussi en PDF.
- **[Closer to Van Eyck](http://closertovaneyck.kikirpa.be) (KIK-IRPA).** Rapport de conservation-restauration interactif du Retable de l'Agneau mystique, en gigapixels.
- **[Cranach Digital Archive](http://lucascranach.org).** Fonds mutualisé par les musées conservant l'artiste, ouvert à la contribution des spécialistes pour trancher les attributions : la publication devient un laboratoire transnational (Welger-Barboza 2012).
- **[Rethinking Guernica](http://guernica.museoreinasofia.es/en) (Museo Reina Sofía).** Environ 2 000 documents organisés en constellation non hiérarchique de récits, étiquetés (chronologie, géographie, contexte), autour d'une étude en gigapixels du tableau (lumière visible, UV, IR, rayons X, 3D) et d'une cartographie des altérations.
- **[Sitterwerk](https://www.sitterwerk-katalog.ch/intro) (Saint-Gall).** Matériauthèque et bibliothèque d'environ 30 000 volumes. Le catalogue reproduit l'espace : visite des rayonnages grâce à la RFID, inventaire continu de l'emplacement, rangement sans place fixe. Les consultants constituent des « collections » sur une table de travail interactive ([Werkbank](http://werkbank.sitterwerk-katalog.ch/table/live)), exportables en livret PDF. Le catalogue devient un outil de travail, articulé à un lieu.
- **[Museum für Kommunikation, Berne](https://mfk.rechercheonline.ch/fr/about#info).** Une seule recherche couvre collections, PTT-Archiv et bibliothèques (MuseumPlus). Deux colonnes qui se répondent : « Données » et « Stories » (depuis février 2024). Les résultats indiquent le nombre de notices, d'objets empruntables et exposés. Le catalogue n'est plus séparé de la médiation.
- **[Kunsthalle Bern](https://archiv.kunsthalle-bern.ch/en/search?people_all=5242).** Archive physique et archive en ligne depuis 2018 (centenaire de 1918-2018), organisée par des fils de recherche; correspondance, catalogues, photographies, cartons d'invitation, presse. Le catalogue prolonge le lieu plutôt qu'il ne le remplace; lien avec la documentation d'expositions (Szeemann, *When Attitudes Become Form*, 1969).
- **[SKKG Sammlung digital](https://digital.skkg.ch/de/intro) (Winterthur).** Collection d'environ 100 000 objets, en ligne depuis mars 2025, 63 431 notices au lancement : choix délibéré de tout publier, même avec des informations rudimentaires. Pas de musée : le catalogue est l'accès principal. Plateforme conçue comme Data Hub; enquête auprès des utilisateurs (juin 2025). La publication du prix d'achat sur certaines fiches est à discuter.
- **[Mona](https://webchat.askmonastudio.com/bot/666e1dc9873d86f0d4aadf1285630bdce47f4a67/?appMode=webapp) (agent conversationnel).** À mettre en regard d'Anna (Reims) et de Natalie Potter (Met) : quel rapport entre l'agent et les données du catalogue ? Que peut-il dire que le catalogue ne dit pas, et inversement ?

## 5. Agréger et ouvrir

Les services tiers (Google Arts & Culture, Europeana) agrègent des données depuis des plateformes externes : ils apportent visibilité et interopérabilité, au prix d'une dépendance aux standards des tiers. Ils se situent en aval du catalogue, et non entre la base de gestion et le catalogue.

Quatre plateformes présentent des objets de plusieurs musées, selon trois logiques : agrégation institutionnelle, échange entre musées, indexation externe. **Question** : qui décide de ce qui entre, et avec quelles conditions d'usage ?

- **[Europeana](https://www.europeana.eu)** : données de plus de 2 000 institutions, collectées par un réseau d'agrégateurs qui les vérifient et les enrichissent. Métadonnées publiées en CC0 (Data Exchange Agreement, depuis juillet 2012); conditions de réutilisation des objets indiquées par le champ `edm:rights`. Le *Publishing Framework* (« plus on donne, plus on reçoit ») prévoit quatre niveaux de participation. À discuter : une notice agrégée perd une partie de son contexte institutionnel au profit de l'interopérabilité.
- **[Reciprocal Research Network](https://www.rrncommunity.org/items)** (Museum of Anthropology, UBC) : outil en ligne de réciprocité pour la recherche sur le patrimoine de la côte du Nord-Ouest. Communautés, institutions et chercheur·ses créent des projets, téléversent des fichiers, discutent. La documentation est co-construite avec les communautés d'origine.
- **[Find an Object](https://findanobject.collectionstrust.org.uk/) (Collections Trust)** : plateforme d'objets que les musées cèdent (déaccessionnés), pour au moins deux mois, avec demandes et offres; repris par Collections Trust en 2026. Ce n'est pas un catalogue de collections mais un outil de la procédure SPECTRUM de déaccession et de cession : la donnée sert la gestion et non la diffusion.
- **[The Last Museum](https://lastmuseum.com)** : moteur de recherche sémantique non institutionnel, environ 6 millions d'œuvres (chiffres variables selon la presse). Il indexe des images déjà publiées par les musées, revendique un *fair use* (qui n'est pas une licence) et reconnaît de nombreuses données inexactes. À discuter : qui répond de la qualité, de la provenance, des conditions d'usage ? La recherche sémantique sépare l'image de son contexte de description; les musées ont-ils un droit de regard ?

### Local Contexts et Manaaki Whenua (Aotearoa Nouvelle-Zélande)

La base ouverte [Systematics Collections Data](https://scd.landcareresearch.co.nz/Specimen/CHR%20469903) (spécimens biologiques nationaux) a été en 2023 la première base de biodiversité à appliquer les outils de [Local Contexts](https://localcontexts.org/bc-labels-and-notice-on-manaaki-whenua/) :

- **Notice** (BC, *Biocultural*) : posée par l'institution sur tous les enregistrements (plus de 675 000 spécimens), elle signale que des droits et intérêts autochtones peuvent exister.
- **Étiquette** : posée par la communauté (iwi) pour dire les conditions d'usage. En avril 2023, trois iwi : Te Whakatōhea (1 166 spécimens), Ngāti Maru (860), Te Roroa (3 983).

Les droits font partie de la fiche; l'autorité passe en partie à la communauté, qui étiquette; la condition d'usage est déclarée.

**Question : cette approche est-elle transposable à un catalogue d'art ?** 

## 6. Regards critiques et conclusion

Manovich (*Le langage des nouveaux médias*, repris dans l'anthologie de Ross Parry) voit dans la base de données une forme symbolique, comme Panofsky pour la perspective à la Renaissance. Avec les mises en ligne massives, l'historien de l'art doit acquérir l'habileté de circuler dans des corpus par plusieurs moyens et de regarder les images dans ce contexte renouvelé.

La numérisation promet de dépasser la fragmentation du musée et de ses collections, mais elle crée des tensions entre fonction scientifique documentaire et médiation. La disponibilité immédiate rompt les hiérarchies entre objets et les différenciations temporelles. Seuls les spécialistes savent replacer chaque objet dans le corpus; la promesse d'exhaustivité renforce la perception d'une équivalence des œuvres et d'un stock documentaire. L'autonomie des œuvres reproduites favorise la confusion entre œuvre et document, et un musée virtuel qui prolonge le musée imaginaire de Malraux.

Elle traduit une crise du jugement esthétique : numérisation accompagnant une rationalisation entrepreneuriale du musée (produits dérivés, marketing), avec l'exposition comme pivot (Haskell), la culture événementielle et la « compulsion patrimoniale » à la présentation exhaustive et indifférenciée. Le musée devient une médiathèque de consultation à la demande.

## Bibliographie sélective

- Borgman, Christine L. 1996. « Why Are Online Catalogs Still Hard to Use? ». *JASIS* 47 (7) : 493-503.

- Ferraris, Maurizio. 2021. *Documentalité*. Paris : Éditions du Cerf.

- Getty Foundation. 2017. *Museum Catalogues in the Digital Age: A Final Report on the Getty Foundation's Online Scholarly Catalogue Initiative (OSCI)*. Los Angeles : Getty Foundation. https://www.getty.edu/publications/osci-report/.

- Parry, Ross. 2007. *Recoding the Museum*. London : Routledge.

- Simard, Françoise. 2001. « Les inventaires virtuels : pourquoi et pour qui ? ». *La lettre de l'OCIM* 78.

- Tunkelang, Daniel. 2009. *Faceted Search*. Morgan & Claypool.

- Turner, Hannah. 2020. *Cataloguing Culture*. Vancouver : UBC Press.

- Welger-Barboza, Corinne. 2012. Voir section 7.

- Whitelaw, Mitchell. 2015. « Generous Interfaces for Digital Cultural Collections ». *DHQ* 9 (1).
