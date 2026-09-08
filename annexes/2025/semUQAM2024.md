title: MSL6517-01
description: emchateau UdeM
theme: presentation/theme/remark-dark-em.css
name: inverse
layout: true
class: inverse

---

name: index

class: center middle

# Ouverture et réutilisation des données muséales

### 15 mars 2024 | Emmanuel Château-Dutier (UdeM)

???

L’ouverture et le partage des contenus culturels (open data et open conten) est une question qui anime le secteur muséal depuis de nombreuses années. 

- essayé de m’interroger sur ce que présenteraient les collègues

Mon intervention s’inscrit dans le cadre d’un programme de recherche partenarial financé par le CRSH dirigé par Johanne Lamoureux et intitulé, *Des nouveaux usages des collections dans les musées d’art* dont je dirige l’axe 4 consacré à la collection partagée.

- Partenariat de 7 ans
- 6 institutions muséales partenaires
- 30 aine de chercheurs

La collection partagée : Avec l’ère numérique, la valeur d’une image est moins déterminée par la dynamique original/reproduction qu’à travers sa mise en circulation par le partage (Gunthert 2015). Depuis plusieurs années en Europe, et plus récemment au Canada, le monde muséal envisage à grande échelle l’ouverture des collections comme une manière d’en prendre soin (Hamilton et Saunderson 2017; Sanderhoff et Edson 2014), donnant un nouvel élan à l’étymologie du terme anglais « care » qui sous-tend la fonction de « curator ». Ce nouveau paradigme autorise des formes d’engagement inédites sur les réseaux sociaux pour les institutions culturelles qui mobilisent les publics. Lorsqu’elle est reconnue dans le domaine public, la collection peut désormais faire l’objet de toutes sortes de réappropriations (Drotner et Schrøder 2013; **Casemajor-Loustau** et al. **2017**; Denoyelle 2018). La multiplication des interfaces muséales (API, IIIF, dépôt de données sur Github, etc.) autorise aussi la circulation des œuvres au-delà des murs de l’institution (**Château-Dutier 2019**, **2020**). Dès lors, comment désormais faire collection et rattacher celle-ci à une marque sinon à un lieu muséal ? Il s’agira de dégager, par une série d’enquêtes (Boltanski 2012), la manière dont ces nouveaux usages se distinguent, d’un point de vue ontologique, des usages physiques des collections (Bermès, 2013; Cameron et Kenderdine 2010; Parry 2010; Ronchi 2008; Saou-Dufrêne et Ihadjaden 2013; Welger-Barboza 2001).

Mon intervention sera l’occasion de vous proposer un rapide panorama de certains enjeux actuels de la muséologie numérique à travers le spectre de l’ouverture des contnus culturels ou des *Open GLAM* comme on les appelle en adoptant un regard critique sur les transformations en cours dans le monde muséal et culturel.

---

layout: false

background-image: url(imagesMSL/mimsy-xg-demo.jpg)

.footnote[MimSy]

???

## Les systèmes de gestion des collections

Les métadonnées occupent une place cruciale dans l’environnement numérique des institutions muséales et patrimoniales. Leur production est au cœur des opérations d’inventaire, d’indexation et de classification des collections, mais aussi de leur diffusion sur le world wide web.

- la documentation réside au cœur des fonctions muséales : continuité des collection, inventaire et signalement approprié, régie des œuvres
- fonctions scientifiques de la documentation

Si les **fonctions d’inventaires** ont depuis toujours occupé les institutions muséales, l’informatique documentaire est venue bouleverser leurs pratiques et leurs approches de la documentation depuis déjà une cinquantaine d’années. Avec la généralisation de la micro-informatique au début des années 80, puis l’avènement du world wide web au milieu des années 90, les musées ont engagé de grandes campagnes d’informatisation de leurs collections qui impliquaient leur documentation structurée mais aussi leur numérisation (Parry 2007).

**L’information muséale rassemble pour l’enssentiel en des données descriptives sur les collections.** La production de ces descriptions et leur structuration exigent le recours au savoir spécialisé du muséologue et mais aussi des modèles métiers spécifiques. Il est assez facile de comprendre que l’on ne décrit pas un artefact muséal comme on décrit un livre. **Or, les musées conservent une grande diversité d’artefacts qui sont le plus souvent des *unica*.** En outre, dans nombre de pays, la production de la description muséale s’inscrit dans un cadre normatif et réglementaire fort. Ainsi les enjeux de l’informatique au musée relèvent avant tout d’un problème de représentation des collections.

---

background-image: url(imagesMSL/metadataNoFuture.png)

???

- Pb des silos
- découvrabilité et métadonnées, 
- réutilisation des données

---

# Découvrabilité et interopérabilité

## Découvrabilité 

> Capacité, pour un contenu culturel, à se laisser découvrir aisément par le consommateur qui le cherche et à se faire proposer au consommateur qui n’en connaissait pas l’existence. 

(Observatoire de la culture et des communications du Québec, 2017)

--

## Interopérabilité

> Capacité d’échanger des données entre systèmes multiples disposant de différentes caractéristiques en termes de matériels, logiciels, structures de données et interfaces, avec le minimum de perte d’informations et de fonctionnalité.

Source: BON, Hugo (2016). «Les métadonnées, un enjeu crucial pour la vidéo », INA Global, [En ligne]. [www.inaglobal.fr/numerique/ article/les-metadonnees-un-enjeu-crucial-pour-la-video-8819]. 

???

Deux notions sont donc étroitement liées à la production des métadonnées, ce sont celles de découvrabilité et d’interopérabilité. Toutes deux dépendent largement de la qualité des métadonnées et du partage d’une vision globale du domaine.

**Découvrabilité** 

> Capacité, pour un contenu culturel, à se laisser découvrir aisément par le consommateur qui le cherche et à se faire proposer au consommateur qui n’en connaissait pas l’existence. 

(Observatoire de la culture et des communications du Québec, 2017)

**Interopérabilité**

> Capacité d’échanger des données entre systèmes multiples disposant de différentes caractéristiques en termes de matériels, logiciels, structures de données et interfaces, avec le minimum de perte d’informations et de fonctionnalité.

Source: Bon, Hugo (2016). «Les métadonnées, un enjeu crucial pour la vidéo », INA Global. <www.inaglobal.fr/numerique/article/les-metadonnees-un-enjeu-crucial-pour-la-video-8819>. 

???

Capacité deux systèmes à communiquer entre eux.

Enjeux multiples : interoperabikite technique mais aussi 

---

template: inverse

class: center middle

# Ouverture des données / ouverture des contenus



---

background-image: url(imagesMSL/OpenGLAM-logo.png)

.footnote[https://openglam.org]

???

OpenGLAM was born as an initiative around 2010, when the Open Knowledge Foundation received a grant from the European Commission as part of the DM2E (“Digitised Manuscripts to Europeana”)

## OpenGLAM numérisation des collections, et ouverture des données muséales

### Qu’est-ce qu’être ouvert ?

Les concepts liés à l’accès ouvert naissent à la croisée des domaines informatiques et universitaires.

Historique du mouvement de l’Open Access

- Déclarations sur l’Open Access : the [Budapest Open Access Initiative](http://www.soros.org/openaccess/read.shtml) (Feb. 14, 2002), the [Bethesda Statement on Open Access Publishing](http://www.earlham.edu/~peters/fos/bethesda.htm) (Apr. 11, 2003), the [Berlin Declaration on Open Access](http://www.berlin9.org/about/declaration/index.shtml) (Oct. 22, 2003), the [Lyon Declaration on Access to Informationa and Development](http://www.lyondeclaration.org/) (Aug. 2014), [Public Library of Science (PLoS)](http://www.plos.org/oa/definition.php) (founded in 2000), and [Creative Commons](http://creativecommons.org/licenses/by/2.5/)(founded in 2001)
- Development of open archives: [Open Archives Initiative](http://www.openarchives.org/) (started in October 1999)
- Adoption of open access policies (starting in 2003): [ROARMAP: Registry of Open Access Repository Material Archiving Policies](http://roarmap.eprints.org/)

Mais là où "une veille tradition et une nouvelle technologie avaient convergé pour apporter un bénéfice public sans précédent." (Budapest 2002) Les musées ne pouvaient pas vraiment se réclamer de la même tradition du partage. Dans le domaine artistique particulièrement, la tradition du connoisseurship. Préciosité. En dépit renouveau de la muséologie.

Relever que la déclaration de Berlin du 22 octobre 2003 souhaitait déjà "encouraging the holders of cultural heritage to support open access by providing their resources on the Internet." https://openaccess.mpg.de/Berlin-Declaration

Rennouvelé Déclaration de Lyon sur l’accès à l’Information et au Développement de Lyon 2014

### Les incitatifs internationaux

Politique d’intégration européenne qui dès la fin des années 70s identifie la politique culturelle comme un levier de l’intégration européenne.

Politiques soutenue par l’Organisation Mondiale du Commerce et le G8

#### Développement de grandes banques d’images

[ArtSTOR](http://www.artstor.org) (voir http://www.artstor.org/mission), [The Bridgeman Art Library](http://www.bridgemanimages.com) fondée en 1972 et [Corbis](http://www.gettyimages.ca/?corbis) (fermé le 2 mai 2016 et réuni à Getty Images)

http://www.artstor.org/content/permitted-prohibited-uses

---

## Chronologie de l’Open access

- **1991**, [ArXiv](https://arxiv.org)
- **octobre 1999**, [Open Archives Initiative](https://creativecommons.org)
- **octobre 1999 - 2000**, [Public Library of Science (PLoS)](https://plos.org)
- **2001**, [Creative Commons](https://creativecommons.org)
- **2002**, [Budapest Open Access Initiative](https://www.budapestopenaccessinitiative.org)
- **2003**, [Bethesda Statement on Open Access Publishing](https://web.archive.org/web/20120216091532/https://earlham.edu/~peters/fos/bethesda.htm)
- **2003**, [Berlin Declaration on Open Access](http://www.berlin9.org/about/declaration/index.shtml)
- **2014**, [Lyon Declaration on Access to Informationa and Development](https://www.lyondeclaration.org)

---

## Open Data

- **2004**, [TheyWorkForYou](https://www.theyworkforyou.com)
- **décembre 2007**, Réunion de Sebastopol (Californie) pour définir le concept of open public data. 
- **2009**, conférence TED de Tim Berners-Lee [« The Next Web »](https://www.ted.com/talks/tim_berners_lee_the_next_web)
- **2009**, Barack Obama signe le [Memorandum on Transparency and Open Government](https://obamawhitehouse.archives.gov/the-press-office/transparency-and-open-government), [data.gov](https://data.gov)
- **2010**, [Bibliothèque nationale d’Allemagne (DNB)](https://www.dnb.de), publication de données d’autorités comme données liées
- **2011**, Lancement de l’[Open Government Partnership](https://www.opengovpartnership.org)
- **2011**, [The British National Bibliography](https://bl.natbib-lod.org) ouverture en CC-0, 2,8M de titres
- **septembre 2011**, Conférence des Bibliothèques nationales européennes (CENL)

---

background-image: url(imagesMSL/openData.png)

.footnote[http://opendatainception.io]

???
Le contexte de l’open data

L'open data ou donnée ouverte est une donnée numérique d'origine publique ou privée. Elle peut être notamment produite par une collectivité, un service public (éventuellement délégué) ou une entreprise. Elle est diffusée de manière structurée selon une méthode et une licence ouverte garantissant son libre accès et sa réutilisation par tous, sans restriction technique, juridique ou financière.

L'ouverture des données (open data) représente à la fois un mouvement, une philosophie d'accès à l'information et une pratique de publication de données librement accessibles et exploitables.

Elle s'inscrit dans une tendance qui considère l'information publique comme un bien commun (tel que défini par Elinor Ostrom) dont la diffusion est d'intérêt public et général.
En Europe et dans certains pays, des directives et lois imposent aux collectivités de publier certaines données publiques sous forme numérique.

## Racines académiques

Déclaration internationale sur le libre accès de Budapest qui s'est tenue le 14 février 2002, connue sous l'acronyme BOAI (Budapest Open Access Initiative)

## egouvernement

Historiquement, ce sont les États-Unis qui ont les premiers lancé un large processus de libération des données publiques (obligation légale pour l'État et ses agences) depuis la loi « Freedom of Information Act » de 1966. Mais les facilités offertes par l'Internet lui ont donné un regain d'intérêt de la part du secteur public depuis 2009 7.

Dans le monde, des mesures en faveur de davantage de transparence vis-à-vis des citoyens se multiplient et les données ouvertes apparaissent comme l'un des moyens de satisfaire leur volonté de participer à la vie de la Communauté et d’exercer leur droit d’être informé en associant un principe des externalités positives au principe de la donnée publique considérée comme bien commun.

En Europe, en 2003, la directive 2003/98/CE du Parlement européen et du Conseil du 17 novembre 2003 sur la réutilisation des informations du secteur public (en anglais, directive) dite PSI (Public Sector Information) va dans le même sens.
Les anglais ont une loi Freedom of Information Act qui date de l'an 2000.

En France, ce mouvement rencontre l'intérêt de nombreuses collectivités (un décideur sur deux de collectivité locale interrogé par MARKESS International en 2012, déclarait envisager l’élaboration d’une stratégie “open data” avant 20148).

Politique UK, EU
Tim Berners Lee

---

## « Raw Data Now ! »

<iframe src="https://embed.ted.com/talks/tim_berners_lee_on_the_next_web" width="854" height="480" style="position:absolute;left:0;top:0;width:100%;height:100%" frameborder="0" scrolling="no" allowfullscreen></iframe>


???

[Tim Berners-Lee: The next Web of open, linked data](https://youtu.be/OM6XIICm_qo)

Conférence TED 13 mars 2009

> Il y a 20 ans, Tim Berners-Lee inventait le World Wide Web. Pour son nouveau projet, il construit un web des données, libres et liées, qui pourrait faire aux nombres ce que le web a fait pour les mots, les photos et les vidéos: libérons nos données et redéfinissons la manière dont nous les utilisons ensemble.
>
> 20 years ago, Tim Berners-Lee invented the World Wide Web. For his next project, he's building a web for open, linked data that could do for numbers what the Web did for words, pictures, video: unlock our data and reframe the way we use it together.

février 2009, The next web, conférence TED de Tim Berners-Lee https://www.ted.com/talks/tim_berners_lee_on_the_next_web

Demande partage de données brutes : « Raw Data Now ! »

Puissance des données collectées et stockées dans des bases de données pour répondre à des questions. Souligne importance des données et de leur réutilisation.

Principe du Linked Data

Chacun fait sa part, même petite, mais connecte ensemble des données. Pas question de quantités de données mais le fait de les connecter ensemble. Parallèle avec ce qu’avait précédemment fait avec le web de document.

https://www.ted.com/talks/tim_berners_lee_on_the_next_web?utm_campaign=tedspread&utm_medium=referral&utm_source=tedcomshare

https://www.ted.com/talks/tim_berners_lee_the_year_open_data_went_worldwide?utm_campaign=tedspread&utm_medium=referral&utm_source=tedcomshare

> A TED2009, Tim Berners-Lee a lancé un appel pour "des données brutes, maintenant" - afin que les gouvernements, les scientifiques et les institutions rendent leur données publiques sur internet. A l'université TED en 2010, il montre quelques-uns des résultats intéressants que l'on obtient en reliant les données.

Rapport avec les politiques d’open data

https://www.ted.com/talks/tim_berners_lee_the_year_open_data_went_worldwide?language=fr

7 juillet 2011, UK David Cameron announced the broadening of the publicly available government data with the publishing of key data on the National Health Service, schools, criminal courts and transport. http://data.gov.uk/data cf. https://www.gov.uk/government/news/pm-sets-ambitious-open-data-agenda

---

## 5 étoiles

![img](imagesMSL/5-star-steps.png)

<http://5stardata.info>

???

Tim Berners-Lee, l’inventeur du web et l’initiateur du Linked Data a suggéré un déploiement en cinq étapes pour les données ouvertes (open data).

#### Plusieurs niveaux d’ouverture de données

- données accessibles sur le web
- données accessibles structurées (XSL, etc.)
- données structurées dans un format-non propriétaire (CSV, XML, etc.)
- Utilisation de URI pour identifier les ressources avec RDF
- Les données sont reliées à d’autres formats pour fournir du contexte

Tim Berners Lee. Linked Data. W3C, 2006. https://www.w3.org/DesignIssues/LinkedData.html

---

## Données 5 étoiles

- ★ make your stuff available on the Web (whatever format) under an open license
- ★★ make it available as structured data (e.g., Excel instead of image scan of a table)
- ★★★ make it available in a non-proprietary open format (e.g., CSV instead of Excel)
- ★★★★ use URIs to denote things, so that people can point at your stuff
- ★★★★★ link your data to other data to provide context

Le site http://5stardata.info/en/ propose pour chacune des 5 étapes de l’ouverture des données des exemples et explique les coûts et les bénéfices qui les accompagne. Les données utilisées pour les exemples sont issues de ‘*the temperature forecast for Galway, Ireland for the next 3 days*’.

---

background-image: url(imagesMSL/imagesUsages.jpg)

.footnote[Denoyelle, Martine, Katie Durand, Johanna Daniel, et Elli Doulkaridou-Ramantani. 2018. « Droits des images, histoire de l’art et société ». Programme Images/Usages, Institut national d’histoire de l’art. Fondation de France. https://www.inha.fr/fr/actualites/actualites-de-l-inha/en-2018/rapport-final-du-programme-images-usages.html.]

???

À l’international, de telles initiatives prennent place dans le contexte d’**un mouvement d’ouverture des données publiques** qui s’inscrit plus largement dans le cadre d’accords de l’OMC et qui se sont notamment manifestés en Europe par plusieurs directives traduites dans les droits respectifs de chaque pays ainsi que des programmes de financement spécifiques qui ont largement profité à la numérisation des collections à travers des projets phares à l’échelle européenne comme Europeana. Cette **injonction au partage** intervient donc dans une perspective de circulation des contenus relativement ambiguë puisqu’elle est notamment destinée à alimenter une économie de la connaissance, elle rejoint cependant une forte demande sociale soutenue par un secteur associatif et militant fourni (OKF, SavoirsCom1, Wikipedia, etc.).

**Depuis les années 2000, la production d’état des lieux, s’avère relativement typique de ce mouvement d’ouverture des collections**, souvent désigné sous l’appelation d’Open GLAM. Alors que plusieurs grands musées internationaux ont fait événement depuis le début des années 2010 en s’engageant à rendre largement accessible les données et les contenus de leurs collections, divers census se sont depuis intéressés, non seulement aux licences concernant leur mise à disposition, mais aussi aux formats et aux modalités de publication. 

Les Premiers **grands recensement sur les droits d’auteur servirent en particulier aux historiens d’art à adresser la question, cruciale pour la discipline, de la disponibilité des images d’art** en ligne et des droits de réutilisation appliqués par les musées sur les œuvres du domaine public. Par exemple, grande étude, souvent citée, de Kenneth D. Crews. On peut évidemment aussi évoquer les rapports récurrents de la College art association sur les droits d’auteur. Plus récemment, la quasi absence de musées d’art canadien dans le recensement collaboratif réuni par Douglas McCarty et Andrea Wallace, *The Open GLAM survey*, en dépit d’une invitation à renseigner le tableau Google ayant circulé sur les listes professionnelles, alerte sur le caractère très inégal de ces politiques à travers le monde, particulièrement au Canada. Dernier avatar de cette démarche, le rapport *Images et Usages* commandé par la Fondation de France dont la rédaction a été dirigée par Martine Denoyelle à l’INHA dresse un bilan critique de la disponibilité des contenus muséaux en France. Ce rapport montre que cette question de l’ouverture des contenus culturels reste un combat en France en dépit de directives européennes fortes.

---

background-image: url(imagesMSL/tousPhotographes.png)

## Une demande sociale

???

Une situation dénoncé par beaucoup dans le domaine de l’art.

Fermeture, enclosure.
Copyfraud

Polémique sur la photographie au Musée d’Orsay.
Campagne de Louvre pour tous.

En février 2012, une lettre ouverte était adressée au ministère de la Culture et de la Communication par plusieurs personnalités se réclamant d’associations d’usagers et d’Amis de musées : elles demandaient l'ouverture d'une concertation sur la possibilité, pour les visiteurs, de photographier les œuvres pendant la visite.

À partir du 4 mai 2012, ce groupe a commencé de se réunir en moyenne une fois par mois. Un peu moins d'une dizaine de séances se sont tenues, rassemblant entre 30 et 40 participants à chaque fois.

En juillet 2014, le ministère de la Culture en France annonçait la signature d’une belle charte intitulée « tous photographes ! ». L’enjeu ? Autoriser dans les monuments nationaux la prise de vue des œuvres afin d’en faciliter le partage sur les réseaux sociaux.

Cf. *Louvre pour tous* et charte de la photographie au musée. SavoirsCom1

En la matière, on est loin d’être tiré d’affaire. Même la Bnf qui est relativement libérale sur le partage de ses métadonnées, se réserve toujours en partie la possibilité d’imposer une redevance sur la reproduction à des fins commerciales des contenus qu’elle numérise.

En France, l’institution qui tient la palme de la politique la plus restrictive est actuellement la Réunion des Musées Nationaux (RMN) qui assure pour de nombreux organismes la gestion des droits photographiques. Pour autant, la gestion de cette commercialisation présente un coût et son service photo était malgré tout déficitaire il y a quelques années.

Au Québec, le musée qui a adopté la politique la plus ouverte, sans doute les Musées de la civilisation qui se sont dotés d’un Stratégie numérique ambitieuse qui accorde une large place à l’Open Access.

---

## Une nouvelle donne pour les musées depuis 2012

- **2008**, Sydney’s Powerhouse museum, premier musée à joindre [The Commons](https://www.flickr.com/commons) (Flickr)
- **2012**, Walters Art Museum et Wikipédia
- **2012**, Rijksmuseum 125 000 œuvres libérées (aujourd’hui 650 000) [Rijkstudio](https://www.rijksmuseum.nl/en/rijksstudio)
- **2012**, [NYPL](https://www.nypl.org/research/collections/digital-collections/public-domain)
- **2012**, British Library adopte la Public Domain Mark pour ses manuscrits enluminés
- **juin 2013**, [National Gallery Washington](https://images.nga.gov/en/page/openaccess.html) 25 000 images HD
- **octobre 2013**, Getty Research Institute 10 0000 images libérées *(aujourd’hui 110 000)*
- **décembre 2013**, British Library 1M images sur Flickr
- **2016** MOMA
- **2017**, MET Open Access Initiative
- **2020**, Paris Musées, 150 000 reproduction d’œuvres
- etc.

???

### Choix de grands musées

Le choix de plusieurs collections de grands musées d’ampleur internationale de mettre à disposition leur images sous licence libre a clairement changé la donne.

[http://www.club-innovation-culture.fr/innovation-dans-les-musees-et-lieux-de-patrimoine-en-france-et-dans-le-monde-cahier-des-tendances-2013/](http://www.club-innovation-culture.fr/innovation-dans-les-musees-et-lieux-de-patrimoine-en-france-et-dans-le-monde-cahier-des-tendances-2013/)

« Libre » fût incontestablement l’un des principaux mots clés de 2013.

- Après le Walters Art Museum et son accord avec Wikipedia en 2012 et le Rijksmuseum et ses 125 000 œuvres téléchargeables librement sur son site (notre coup de cœur de l’an dernier),
- En juin 2013, la National Gallery de Washington lançait un nouveau site web et mettait en accès libre 25 000 images en haute résolution (+ 3000 pixels). Le site en contient aujourd’hui 32 000
- En août et octobre 2013, le Getty Research Institute mettait 10 000 images dans son programme de contenus disponibles pour une utilisation sans restriction.  (Avec 5 400 images supplémentaires, Getty double son volume de contenus libres disponibles en ligne  L’institut Getty met en accès libre près de 4 700 œuvres numérisées de sa collection)

Présentation vidéo du programme Open Content du Getty
http://www.youtube.com/watch?v=v4xJCjOcoWk

- Le mercredi 13 novembre 2013, la Smithsonian Institution, le plus grand complexe muséal aux USA et dans le monde, a lancé une nouvelle visionneuse 3D en ligne, qui permet au public de manipuler des centaines objets en 3D. Les données peuvent également être téléchargés et reproduites avec une imprimante 3D. Sur les plus de 130 millions d’objets dans ses collections, 14 millions sont déjà choisis pour être numérisés (Les objets du Smithsonian peuvent désormais être imprimés en 3D à domicile  Dans un e-book, le patron de la Smithsonian Institution explique sa stratégie numérique et mobilise les musées du monde)

Cette déferlante de contenus libres d’utilisation a même inspiré un article à la Une du NY Times en mai 2013 intitulé « les œuvres d’art pour un et pour tous »

Même si le Rijks qui lance le mouvement 125 000 œuvres téléchargeables publiées en 2012

Pour des raisons juridiques et stratégiques, ce mouvement de l’open est essentiellement américain, cependant le mouvement fait également son chemin en Europe

- en mars 2013, la bibliothèque nationale des Pays Bas annonçait la mise en accès libre d’une partie de ses collections de manuscrits et de journaux et magazines anciens.
- la BNF, en novembre 2013, décidait de mettre ses métadonnées descriptives en licence ouverte.
- Et en décembre 2013, la British Library postait 1 million d’images de sa collection sur Flickr. (La British Library met en ligne sur Flickr plus d’un million d’illustrations libres de droit)

C’était un début !

[http://www.museum-id.com/idea-detail.asp?id=389](http://www.museum-id.com/idea-detail.asp?id=389)

[http://www.openculture.com/2016/03/the-museum-of-modern-art-moma-puts-online-65000-works-of-modern-art.html

### LACMA

Nearly 20,000 images of artworks the museum believes to be in the public domain are available to download on this site. Other images may be protected by copyright and other intellectual property rights. By using any of these images you agree to LACMA’s [Terms of Use](https://www.lacma.org/about/contact-us/terms-use).

 (1) images of works from LACMA’s collections that LACMA believes are in the public domain, some of which are made available without restriction (these images are marked "Public Domain High Resolution Image Available" as described below); or (2) protected by copyright (the "Protected Content"). Such Content, whether or not in the public domain, may be subject to other restrictions as well, including rights of privacy and publicity, under applicable law.

### GLAM collections

Galleries, Libraries, Archives, and Museums

- Archives of American Art, [http://www.aaa.si.edu/](http://www.aaa.si.edu/).
- Cleveland Museum of Art, Research Image Catalog, [http://library.clevelandart.org/search_images](http://library.clevelandart.org/search_images)
- Getty Open Content: [http://www.getty.edu/about/opencontent.html](http://www.getty.edu/about/opencontent.html)
- Metropolitan Museum of Art, [http://www.metmuseum.org/collection/the-collection-online](http://www.metmuseum.org/collection/the-collection-online)
- Museum of Modern Art, [http://www.moma.org/collection/advancedsearch.php](http://www.moma.org/collection/advancedsearch.php)
- Museo Nacional del Prado, [https://www.museodelprado.es/coleccion/galeria-on-line/](https://www.museodelprado.es/coleccion/galeria-on-line/)
- NGA Images, [https://images.nga.gov/en/page/show_home_page.html](https://images.nga.gov/en/page/show_home_page.html)**Table 3**
- Te Papa Tongarewa, Museum of New Zealand, [http://collections.tepapa.govt.nz](http://collections.tepapa.govt.nz/)/
- Victoria and Albert Museum, [http://collections.vam.ac.uk/](http://collections.vam.ac.uk/)
- Walters Art Gallery, [http://art.thewalters.org/](http://art.thewalters.org/)

cf. Kelly 2013, p. 23-24

Question de la perte du contrôle intellectuel et des visites soulevées mais peu démontrées.

### Une chronologie du contenu ouvert dans les musées

2014

> A few weeks ago we [released an updated version](https://blog.tepapa.govt.nz/2014/02/26/updated-collections-online/) of Collections Online, making images bigger, search results clearer,  and easier to use regardless of what device you are using. Today we are  extremely happy to let you know about our latest development; over **30,000 images downloadable, for free, in the highest resolution we have them**. You can search for and download them at [Collections Online. ](https://collections.tepapa.govt.nz/)

https://blog.tepapa.govt.nz/2014/06/03/free-downloadable-images-from-te-papas-collections/

cf. https://wiki.creativecommons.org/index.php/GLAM

https://blog.tepapa.govt.nz/2016/03/01/get-downloading-20-great-glam-websites-for-free-high-resolution-imagesMSL/

---

## La notion de communs culturels

> **Bien communs.** Toute « chose » ou entité immatérielle à laquelle on a décidé de donner un statut de propriété commune, de la faire appartenir à tous, parce qu’elle n’appartient à personne. Dans le sens moderne, la propriété commune est universelle, elle est celle de l’humanité. Dans le sens ancien, il s’agissait souvent de la propriété d’une communauté restreinte. À ne pas confondre avec les biens publics dans le sens d’objets d’une propriété publique (gérée par des institutions publiques).

(Aigrain 2005, p. 265)

--

> **Biens communs informationnels.** Bien communs qui peuvent être créés, échangés et manipulés sous forme d’information, et dont les outils de création et le traitement sont souvent eux-mêmes informationnels (logiciels). Il peut s’agir de données, de connaissances, de créations dans tous les médias, d’idées, de logiciels. Les biens communs informationnels sont des biens publics parfaits au sens économique, contrairement aux biens communs physiques, qui gardent toujours une part de rivalité ou d’excluabilité.

(Aigrain 2005, p. 265)

---

## Contenus ouvertes et domaine public

- « Définition du Savoir Libre ». s. d. Open Knowledge Foundation. Consulté le 10 janvier 2020. https://opendefinition.org/od/1.1/fr/.
- Definition of Free Cultural Works https://freedomdefined.org/Definition
- « Public Domain Manifesto ». 25 janvier 2010. COMMUNIA. https://publicdomainmanifesto.org/manifesto/#fr.

Parallèle avec le logiciel libre et open source

- « Définition du logiciel libre ». s. d. gnu.org. Consulté le 11 janvier 2020. https://www.gnu.org/philosophy/free-sw.html.
- « The Open Source Definition ». 1999. Open Source Initiative. https://opensource.org/docs/osd.

---

## The Public Domain Manifesto (2010)

« Public Domain Manifesto ». 25 janvier 2010. COMMUNIA. https://publicdomainmanifesto.org/manifesto/#fr.

>Le domaine public structurel est au cœur de la notion de domaine public : il comprend tout notre savoir commun, notre culture et les ressources qui peuvent être utilisées de par la loi actuelle sans restriction liée au droit d’auteur. Plus précisément, le domaine public structurel a deux composantes :
>
>1. **Les œuvres dont la protection a expiré.** [...]
>
>2. **Les biens communs informationnels essentiels qui ne sont pas couverts par le droit d’auteur.** [...]
>
>Le domaine public structurel a été construit dans l’histoire pour contrebalancer les droits protégés par le droit d’auteur. Il est essentiel à la mémoire culturelle et aux savoirs fondamentaux de nos sociétés.

???

Le *Public Domain Manifesto* est un manifeste qui fut produit dans le cadre de l’association européenne pour le domaine public COMMUNIA. L’idée de ce manifeste émerge à l’occasion de la première conférence COMMUNIA. Plusieurs mois de travail permirent l’élaboration d’un premier brouillon qui circula ensuite parmi les membres de l’association avant d’être rendu public le 25 janvier 2010.

---

background-image: url(imagesMSL/openGlamSurvey.png)

.footnote[Douglas McCarthy et Andrea Wallace, Survey of GLAM open ac cess policy and practice, 2018- *https://t.co/pBqry2klmk*]

---

template: inverse

class: center middle

# Exemples de réemplois et de réutilisation

???

Mise en œuvre de l’ouverture

---

background-image: url(imagesMSL/rijkstudio.png)

https://www.rijksmuseum.nl/en/rijksstudio

???

L’exemple du Rijksmuseum

En 2013, le Rijksmuseum a rouvert ses portes après une période de rénovation de 10 ans. Rôle du site important pour communication. Nouveau site présenté au public le 30 octobre 2012. 

Ce projet, lancé en attendant la réouverture du musée pour le 13 avril 2013, a constitué une sorte de révolution dans le secteur muséal. À l’inverse du Centre Pompidou Virtuel, qui fait la part belle au texte et à la recherche sémantique, le Rijksmuseum a souhaité privilégier l’image.

> « La mission du Rijksmuseum est de connecter le public, l’art et l’histoire » souligne Peter Gorgels. Bref, avec Rijksstudio, le Rijksmuseum voulait créer une expérience esthétique.

Repose sur une numérisation large. 125 000 oeuvres offertes à tous ! au moment de l’ouverture.
Un autre grand part pris a été d’offrir librement aux visiteurs de partager, modifier, télécharger, créer à partir des collections numérisées.

Ouverture une valeur fondamentale du site. 125 000 images libres de droit.
Rijksstudio encourage leur téléchargement et leur réutilisation.



Plus de deux ans après son lancement, le Rijksstudio était toujours cité en exemple pour l’ouverture maximale de ses collections. Quel est le bilan de ce nouveau modèle ? Quels en sont les développements futurs.

Martijn Pronk rejoint le musée en 2007, développé et participé au lancement du nouveau site reposant sur une politique maximale d’ouverture de ses collections.

> Martijn Pronk (Rijksmuseum): «Le Rijksstudio a attiré quelques 15 millions de visites pour 200 000 comptes personnels créés»

> « Avec le Rijksstudio, le Rijksmuseum a pu donner accès à sa collection gratuitement et s’ouvrir vraiment : chaque visiteur est désormais le directeur de son propre musée. »

Près de deux ans et demi se sont écoulés depuis le lancement du Rijksstudio. Le nombre d’images disponibles atteint maintenant presque 200 000, et chaque jour de nouvelles reproductions d’œuvres viennent les compléter.

Le site web a attiré quelques 15 millions de personnes pour 200 000 Rijksstudios personnels créés à ce jour. Ces derniers incluent presqu’un demi-million de collections personnelles.
Plus d’1,3 million d’images ont été téléchargées pour un usage privé ou commercial, soit environ 1.400 par jour en moyenne.

> « Le Rijksmuseum a mis sa collection à la portée du public par conviction. Nous partons du principe que la collection n’est pas notre propriété personnelle. Elle appartient à tout le monde ! C’est pourquoi nous encourageons activement chacun à l’utiliser. »

### Une stratégie qui s’inscrit dans une stratégie numérique globale

Le Rijksstudio découle directement de la stratégie numérique du Rijksmuseum, dont un des aspects importants est la mise à disposition de notre contenu. 

Pensent qu’il est possible d’atteindre les différents publics là où ils se trouvent, en utilisant les moyens et supports les plus adaptés.

Wikipedia en est un bon exemple. Le Rijksmuseum ne produit pas de contenus sur cette plateforme, mais nous le musée a placé toutes ses images dans Wikimedia Commons, afin de permettre ainsi aux Wikipédiens d’utiliser eux-mêmes le contenu. Cela leur évite d’avoir à mettre à jour les informations moins demandées. Celui qui veut avoir des informations sur Rembrandt visitera très probablement notre site. Mais celui qui cherche des informations sur le peintre Coeman, beaucoup moins connu, pourra se rendre plutôt sur Wikipedia.

### Usages favorisés

Quels types d’usages souhaitez-vous favoriser avec le Rijksstudio?

Les musées sont encore très souvent orientés sur « l’émission d’informations ». Ils doivent gérer énormément de contenu et proposer un grand nombre de produits et services différents. Le Rijksmuseum crée les conditions permettant aux gens de se servir des images comme bon leur semble.

Mais pour cela, le contenu doit être le plus neutre, et donc le plus réutilisable possible. Au lieu d’avoir à tout reprendre à zéro avec chaque nouveau produit ou service, nous devons utiliser autant que possible ce qui a déjà été développé. La mise à disposition de notre contenu permet à d’autres utilisateurs ou prestataires de s’en servir pour développer des créations personnalisées. Ceci illustre bien ma position selon laquelle le libre accès est un moyen et non un objectif.

Comme je l’ai déjà dit, l’ouverture est une valeur fondamentale importante du Rijksmuseum. Sur le site Web, cette ouverture se retrouve dans la proximité de la collection. La collection est à portée de main. Le site Web repose sur la puissance de l’image : « l’image est l’interface ». Maintenant que nous avons mis le contenu à disposition, chacun peut s’en rapprocher. En téléchargeant des images, mais aussi en rassemblant et en partageant ses œuvres préférées avec des amis. En téléchargeant des détails d’images. Mais surtout en créant de nouvelles œuvres uniques à partir des images du Rijksmuseum.

Ceux qui rassemblent des objets dans leur propre Rijksstudio ajoutent une partie d’eux-mêmes au Rijksmuseum. Les collections sont intégrées dans le moteur de recherche, et les plus belles sont présentées sur une page d’accueil. Beaucoup d’entre elles sont des sélections surprenantes d’éléments de notre collection. La façon dont nos visiteurs organisent leurs collections est totalement différente de celle du musée lui-même. Ensemble, les visiteurs et utilisateurs du Rijksstudio permettent au Rijksmuseum de rester en permanence actuel, surprenant et inspirant.

http://www.club-innovation-culture.fr/martijn-pronk-rijksmuseum-le-rijksstudio-a-attire-quelques-15-millions-de-visites-pour-200-000-comptes-personnels-crees/



Comme son nom le laisse deviner, même si vous ne parlez pas un mot de flamand, le Rijksstudio est une application numérique innovante qui rend une (très) grande partie des collections du musée disponibles à tous et ce… gratuitement. Cela veut dire qu’en fait 125 000 oeuvres entièrement numérisées et disponibles en haute définition (bien plus haute que celle proposée par le Google Art Project) sont téléchargeables par tout-un-chacun pour en faire ce que l’on veut et absolument ce que l’on en souhaite.

C’est ainsi que le musée, pour le lancement de ce projet, a fait appel à de grands artistes lors d’une « campagne d’ambassadeurs ». Des petites installations éphémères du Rikjsstudio naissaient dans différents lieux comme dans le magasin De Bijenkorf, installations dans lesquelles les visiteurs étaient invités à réaliser leurs propres chefs d’oeuvre.

ex. Tatouage par Droog, basé sur la peinture du XVIIe "Still Life with Flowers" de Jan Davidsz. de Heem

ex. Foulard en soie d'Alexander van Slobbe basé sur les collections du Rijksmuseum

Que ce soit le Rijksstudio ou le site web du Rijksmuseum, tous deux ont été développés sur le principe des applications, c’est-à-dire permettre au visiteur de trouver rapidement de l’information avec le minimum d’interaction et de parcours. Et, est-il nécessaire de le dire, le site est également complètement responsive (adapté aux différents supports mobiles).

Le Rijksstudio  et le nouveau site du Rijksmuseum ont tous les deux vu le jour grâce à une prise de conscience de la part du personnel du musée sur les comportements de leur public. Aujourd’hui, nous nageons dans un « océan d’images », selon les mots de Peter Gorgels. Particuliers comme organisations publient et partagent leurs images, leurs contenu sur des réseaux sociaux comme Facebook, Flickr, Instagram et Twitter. Cette nouvelle consommation d’images a conduit également les industriels à penser et à créer les tablettes qui offrent un support de qualité pour la visualisation des images et des vidéos.
Le nouveau site est également parti d’un constat sur les musées dits « virtuels » actuels, qui ne sont souvent aujourd’hui que des plateformes, des photothèques d’oeuvres à la navigation mal aissée et souvent aux restrictions poussées en ce qui concerne le partage ou le téléchargement. Ces bases de données n’étant pas vraiment tournées vers le public, elles n’ont donc rencontré que peu de succès. Ce constat couplé au fait que les visiteurs sont amenés très facilement à changer de support de navigation (tablette, smartphone, ordinateur portable, etc.) et qu’ils aiment naviguer simplement, rapidement et consomme des images a rapidement conduit l’équipe de Peter Gorgels à penser en mode « app ».

Qu’est-ce que cela veut dire ? Tout simplement que les applications ont été pensées pour être simples d’utilisation. Elles offrent, mine de rien, assez peu de services, mais ceux-ci sont toujours pertinents. Il fallait donc faire en sorte que l’information, constituée en forme de millefeuille, puisse être accessible rapidement.
125 000 oeuvres offertes à tous !

Un autre grand part pris a été d’offrir librement aux visiteurs de partager, modifier, télécharger, créer à partir des collections numérisées.
La fermeture du bâtiment principal pour rénovation a été l’occasion pour le musée de numériser une grande partie de ses collections. En effet, comme beaucoup, seule une partie des collections (8 000 sur 1 100 000 d’oeuvres) sera exposée au public dans le nouveau Rijksmuseum. Ce dernier a donc décidé qu’elles devaient être accessibles à tous et ce, gratuitement. Au-delà du principe d’open content (Anderson, 2009) qui stipule que, puisqu’il est aujourd’hui possible de distribuer très facilement du contenu, l’avis général est de le rendre  accessible à tous, libre de tout droits d’auteurs (attention, cela ne veut pas dire que c’est libre de droits), le musée a décidé d’investir le champ de l’open design.

http://culture-communication.fr/fr/rijksstudio-faites-ce-que-vous-voulez-des-grands-maitres-flamands/

http://rijksmuseum.github.io

---

background-image: url(imagesMSL/rijkstudio02.jpg)

.footnote[Belarusian designer Lesha Limonov scooped the 2017 Rijksstudio Award with his ’Never Sleep’ eye mask (Image credit: Limonov scooped)]

---

background-image: url(imagesMSL/rijksAPI01.png)

.footnote[<https://github.com/search?utf8=✓&q=Museum&type=Users&ref=searchresults>]

---

background-image: url(imagesMSL/statistiques.png)

.footnote[Artistes femmes dans la collection du MAC (1964-2020), https://observablehq.com/@artistes-femmes-mac]

---

background-image: url(imagesMSL/europeana.png)

.footnote[https://www.europeana.eu/portal/fr]

???

## Agrégation sémantique

The European Digital Library lancée en 2008 pour rendre accessible le patrimoine culturel Européen à travers un point d’accès unique. Sa création fut initiée par une lettre d’intention de six chefs d’État et de gouvernement à la Commission en 2005.

cf. Commission européenne (2014). Timeline of digitisation and online accessibility of cultural heritage. https://ec.europa.eu/digital-single-market/en/news/timeline-digitisation-and-online-accessibility-cultural-heritage

- mise en place d’un accès unifié à plus de 2 millions d’artefacts numérisés en novembre 2008. Bénéficie de l’effort déjà largement engagé dans chacun des pays concernés.
- en 2010, déjà bien au-delà de 6 millions d’artefacts numérisés envisagés, avec 10 millions.
- en 2018, 3700 institutions impliquées (bibliothèques, musées, archives, collections audiovisuelles) offrant un accès commun multilingue à plus de 58 millions de ressources en ligne ! 
  (cf. https://eur-lex.europa.eu/legal-content/EN/TXT/PDF/?uri=COM:2018:612:FIN&from=EN)

Initiative commune qui a servi de modèle à la création d’une initiative américaine comparable, la Digital Public Library of America (DPLA) <https://dp.la>.

---

background-image: url(imagesMSL/nomisma.png)

.footnote[Nomisma <http://nomisma.org>]

---

background-image: url(imagesMSL/crotos.png)

.footnote[http://zone47.com/crotos]

???

Crotos est un moteur de recherche et d’affichage d’œuvres d’art s’appuyant sur Wikidata et Wikimedia Commons.

- 216 897 œuvres, dont 118 870 avec image HD
- Liens vers Wikipédia , sites de référence – multilingue – libre Domaine publicCC 0AttributionPartage dans les mêmes conditions – Lab

http://zone47.com/dozo/crotos-moteur-de-recherche-sur-les-oeuvres-dart-dans-wikidata

---

background-image: url(imagesMSL/lux.png)

.footnote[Lux https://lux.collections.yale.edu]

---

background-image: url(imagesMSL/sari.png)

.footnote[[Bilder Der Schweiz Online](https://bso.swissartresearch.net/)]

---

background-image: url(imagesMSL/Logo_Stacked.png)

## Le cadre international d’interopérabilité des images (IIIF)

*IIIF, prononcer « triple-EYE-eff »*

.footnote[https://iiif.io/demos/]

???

IIIF et l’interopérabilité des images

*L’International Image Interoperability Framework* (IIIF) réunit un ensemble de normes techniques qui facilitent la publication de contenus patrimoniaux sur le web en s’appuyant sur des outils standardisés. Adopté par de nombreuses institutions patrimoniales à travers le monde, ce protocole est encore peu mobilisé au Canada et au Québec. Les collaboratoires du partenariat *Des nouveaux usages des collections dans les musées d’art* seront consacrés en 2024 à l’exploration des riches possibilités offertes par ce protocole d’interopérabilité pour la valorisation et l’éditorialisation des collections d’art. À travers quatre séances collaboratives, les principes généraux du protocole, ses différentes briques technologiques, et de nombreux exemples d’application dans le secteur muséal seront présentés ainsi que des logiciels libres et facilement utilisables pour démontrer l’intérêt de IIIF et favoriser son adoption parmi les musées partenaires.

IIIF est un ensemble de normes ouvertes permettant de fournir des objets numériques de haute qualité ainsi que leur attribution à grande échelle. C’est aussi une communauté internationale qui développe et met en œuvre les API de IIIF. IIIF est soutenu par un consortium d’institutions culturelles de premier plan.

Ces normes et standards sont destinés à assurer :

- une interopérabilité des images
- la création de standards pour diffuser les images
- le développements d’outils basés sur ces standards (serveurs d’images, visionneuses, outils d’annotation, création d’expositions numériques)

IIIF propose des modèles pour présenter et annoter des contenus numériques (images et fichiers audiovisuels), mais c’est aussi une communauté qui développe des APIs ouvertes et implémente des outils qui consomment ces APIs sur le web. Une communauté vivante et dynamique. 

---

background-image: url(imagesMSL/mirador.jpg)

.footnote[International Image Interoperability Framework http://iiif.io, http://projectmirador.org]

---

background-image: url(imagesMSL/biblissima.png)

.footnote[Démo de reconstitution virtuelle du manuscrit 5 de Châteauroux https://demos.biblissima.fr]

---

background-image:url(imagesMSL/aries-interface2.png)

.footnote[[ARIES: ARt Image Exploration Space](http://artimageexplorationspace.com/)]

---

## Research Space

http://www.researchspace.org

https://latehokusai.researchspace.org/resource/rsp:Start

???

Partant d’une source, on procède à sa description, puis on met en place des outils accessibles aux historiens d’art pour **offrir une navigation efficace et proposer des manipulations automatisées sous la forme de visualisations ou de descriptions synthétiques**, à même d’alimenter des discours historiques conformes aux canons de la discipline.

fig

C’est que le numérique n’est pas totalement dépourvu de matérialité, il convient donc **d’être attentif à l’inscription physique des activités intellectuelles dans l’interface** et à la manière dont elles sont révélées (ou transformées) par ce déplacement. 

Ce que l’on cherche à produire avec cette édition c’est un **dispositif d’interprétation**. C’est à ce titre que l’on peut légitimement parler de la **production d’une lecture instrumentée.**

---

## Conclusion

???

À bien des égards, on peut dire que la plateforme Europeana est caractéristique de la Convergence musée bibliothèque. Une convergence dont est directement issu l’acronyme GLAM pour Gallery, Libraries, Archives et Bibliothèque. Plusieurs publications envisagent à partir des années 90 cette convergence à l’instar de Corinne Welger Barboza avec son *devenir médiathèque du musée*. La culture open source des nouveaux médias signifie des interfaces ouvertes, la liberté de se connecter à des images techniques. D’une certaine manière même le code informatique constitue une sorte d’interface. On assiste donc à la multiplication des interfaces déployées par les musées pour la mise à disposition des données de leur collection. Parfois par l’intermédiaire d’Interface programmable (cad accessible à des client informatiques par voie programmatique) parfois sous la simple forme de Dump de données sur GitHub. Ces évolutions s’accompagnent parallèlement de l’apparition d’un nouvel environnement logiciel avec des protocoles tels que IIIF pour le partage d’images, la création d’APIs informatiques et surtout d’outils pour les consommer qui tirent parti des services ainsi constitués.

Avènement possible d’une nouvelle conceptualisation des musées

En 1991, dans un article intitulé *The museum as “information utility”*, George MacDonald et Stefen Alsford expliquent que traditionnellement les musées ont focalisé leur attention sur le passé (MacDonald et Alsford 1991). Leur préoccupation à l’égard des restes matériels du passé explique en partie leur focalisation sur les objets. Une orientation que reflète l’énumération des diverses définitions traditionnellement associées au musées : collectionnent, préservation, étude, exhibition, interprétation. Un ensemble d’activités qui se pratiquent généralement sur site. D’après les auteurs, cette «  focalisation introvertie  » a en quelque sorte convaincu les musées que leur raison d’être était leurs collections d’artefacts plutôt que de la considérer comme un outil à travers lequel nous apprenons à propos du passé. Ce qui explique aussi largement que les musées aient acquis l’image d’institutions caractérisées par les interdictions, archivant les reliques d’un passé mort, seulement accessible à une élite esthétique ou intellectuelle (MacDonald et Alsford 1991).

Dans cet article, qui paraît après-coup particulièrement visionnaire compte tenu des développements récents de la muséologie mondiale, les auteurs proposaient de ne plus seulement servir la collection, mais la société. Selon eux, l’évolution du contexte social et politique, tout autant que de celle des technologies justifiaient déjà que les institutions répondent mieux aux besoins informationnels de la société. Et de réclamer d’envisager le musée dans la perspective non pas strictement de ses fonctions, mais de ses produits.

- génération d’informations résultant d’activité de recherche
- perpétuation d’informations sur les collections
- l’organisation des relations entre des éléments discrets d’information, y compris la recontextualisation d’artefact
- la dissémination

**Cadre d’opération global**, théorie d‘opération unifiante reflétant le cycle de vie de l’information à travers l’ensemble des départements du musée.

**Rôle d’interface du musée entre le visiteur et l’objet identifié depuis longtemps** (édito Museum Management and Curatorship, 1990)

**Montrer que cette conception, même si elle est fondamentalement néolibérale dans son énonciation, rejoint très directement celle de l’imputabilité sociale des musées qui agite actuellement les institutions.**

Directeurs de grands musées interviewés sur l’avenir des musées au Canada en 2016 {Maguire 2016} Tous signalent l’engagement avec le public et rôle communautaire, la demande d’une autorité partagée. http://canadianart.ca/features/whats-the-future-of-canadas-museums/ Question de la démocratisation associée au fait de rendre le patrimoine numérisé accessible à tous. L’avènement des technologies a rendu le patrimoine de plus en plus pluraliste et moins dépendant des experts (Witcomb 2007)

La solution n’est donc non pas technique mais fondamentalement politique. Ce n’est pas un fait nouveau, et on sait tous combien le fait de disposer d’une image ne suffit pas à autoriser sa réutilisation. Mais au-delà des strictes questions d’autorité à laquelle permet notamment de répondre la mise à disposition d’interfaces programmables, pour les images la question fondamentale reste en grande partie politique. Que deviennent alors dans ce nouvel environnement logiciel les possibilités d’engagement avec les collections mais également que deviennent dans ce contexte les collections. Dès lors comment continuer à faire musée ? Où est le musée s’il est partout ou bien s’il devient distribué ?

- Quelles possibilités engagement avec collections.
- Que deviennent dans ce contexte les Collections ?
- Où peut-être le musée, s’il est partout ?

Avènement du musée imaginaire.

Dès lors comment continuer à faire musée ? **Où est le musée s’il est partout ou bien s’il devient distribué ?** Quelles éditorialisations possibles ?

Si l’on souhaite réellement voir ce genre d’interfaces se multiplier, il me semble impossible de seulement se focaliser sur la question des licences et des droits. On ne pourra pas faire l’économie d’une réflexion sur les conséquences pour les musées sur leur représentation et l’identité de leurs collections.

Il s’agit donc de comprendre ce qui peut accompagner cette évolution des musées comme service informationnel en faisant en sorte que ce modèle puisse s’aligner avec les valeurs portées par l’institution et le projet d’établissement.

Ne pas ignorer les risques de dissolution de l’identité des collections.

Prendre conscience des tensions en jeu dans les institutions pour faire avancer la belle promesse d’un accès riche et généralisés aux œuvres des collections qui est à portée de main. 





## Une généalogie de l’ouverture

Au cours de la dernière décennie, nombre de musées d’art européens, rapidement rejoints par plusieurs grands musées américains, se sont fortement engagés dans **un processus d’« ouverture de leurs collections »** qui s’est traduit par la mise à disposition des informations documentaires mais aussi la publication des images des œuvres qu’ils conservent et leur diffusion en ayant recours à des licences libres. La situation à l’égard de ce qu’on appelle couramment l’Open GLAM fait l’objet d’une veille soutenue par une forte mobilisation des publics, particulièrement en Europe. 

Il ne s’agit pas tant ici d’évoquer les catalogues en ligne de musées, leurs applications pour terminaux mobiles, ou les déploiement d’expositions virtuelles, mais plutôt les stratégies de partage de contenus, l’adoption de licences libres et ou encore les formes plus spécifiques à l’informatique comme la mise à disposition de jeux de données, ou la création d’interfaces programmables dans lesquelles sont actuellement engagés nombre de musées ou d’institutions culturelles.

À l’international, de telles initiatives prennent place dans le contexte d’**un mouvement d’ouverture des données publiques** qui s’inscrit plus largement dans le cadre d’accords de l’OMC et qui se sont notamment manifestés en Europe par plusieurs directives traduites dans les droits respectifs de chaque pays ainsi que des programmes de financement spécifiques qui ont largement profité à la numérisation des collections à travers des projets phares à l’échelle européenne comme Europeana. Cette **injonction au partage** intervient donc dans une perspective de circulation des contenus relativement ambiguë puisqu’elle est notamment destinée à alimenter une économie de la connaissance, elle rejoint cependant une forte demande sociale soutenue par un secteur associatif et militant fourni (OKF, SavoirsCom1, Wikipedia, etc.).

**Depuis les années 2000, la production d’état des lieux, s’avère relativement typique de ce mouvement d’ouverture des collections**, souvent désigné sous l’appelation d’Open GLAM. Alors que plusieurs grands musées internationaux ont fait événement depuis le début des années 2010 en s’engageant à rendre largement accessible les données et les contenus de leurs collections, divers census se sont depuis intéressés, non seulement aux licences concernant leur mise à disposition, mais aussi aux formats et aux modalités de publication. 

Les Premiers **grands recensement sur les droits d’auteur servirent en particulier aux historiens d’art à adresser la question, cruciale pour la discipline, de la disponibilité des images d’art** en ligne et des droits de réutilisation appliqués par les musées sur les œuvres du domaine public. Par exemple, grande étude, souvent citée, de Kenneth D. Crews. On peut évidemment aussi évoquer les rapports récurrents de la College art association sur les droits d’auteur. Plus récemment, la quasi absence de musées d’art canadien dans le recensement collaboratif réuni par Douglas McCarty et Andrea Wallace, *The Open GLAM survey*, en dépit d’une invitation à renseigner le tableau Google ayant circulé sur les listes professionnelles, alerte sur le caractère très inégal de ces politiques à travers le monde, particulièrement au Canada. Dernier avatar de cette démarche, le rapport *Images et Usages* commandé par la Fondation de France dont la rédaction a été dirigée par Martine Denoyelle à l’INHA dresse un bilan critique de la disponibilité des contenus muséaux en France. Ce rapport montre que cette question de l’ouverture des contenus culturels reste un combat en France en dépit de directives européennes fortes.

#### Historiciser la question

Il faut d’abord bien avoir à l’esprit qu’il existe en quelque sorte **une généalogie de l’ouverture des collections**. Cette généalogie prend probablement sa source dans l’important renouveau qu’ont connu les musées depuis la fin des années 70, sous l’influence de la nouvelle muséologie puis du tournant managériales des musées qui ont profondément renouvelé leurs opérations et leurs rapports avec le public. Depuis les années 80, nombre d’institutions se sont ainsi investies dans de nouvelles politiques de public et cherché à animer leurs collections en ayant largement recours à des approches innovantes, notamment dans les musées de sciences. Lorsqu’elles étaient techniques, ces innovations ont aussi largement bénéficié depuis la fin des années 70 et au début des années 80 de forts incitatifs financiers destinés à soutenir l’émergence d’un secteur industriel des nouvelles technologies de l’information. On peut notamment affirmer – c’est le cas pour la France mais également probablement dans de nombreux pays – que le secteur muséal et culturel a bientôt été identifié comme un domaine d’expérimentation. Ce contexte explique largement les premières entreprises de numérisations patrimoniales développées à partir de la fin des années 70 et qui ont directement servi à mettre au point des standards de numérisation et de traitement des images par l’informatique. Les politiques européennes culturelles étant en ce sens venues prolonger ce mouvement initial en inscrivant leur financement dans le cadre de politiques de soutien à l’innovation avec différents programmes spécialisés puis des grandes appels à projets comme Horizon 2020, etc.

Ainsi que l’avait rapidement identifié Jacques Thuillier, l’avènement du word wide web au milieu des années 90 allait fournir **un débouché relativement évident pour les produits issus de ces premières campagnes de numérisation patrimoniales**. La plateforme du web se caractérise en effet par son caractère multimédia et qu’elle permet une diffusion large et facile des images. Ainsi, les musées ont-ils multipliés, depuis le début des années 2000, la publication de leurs catalogues en ligne à partir de leur systèmes d’information. Ce faisant, les musées ont constitué d’importantes ressources non seulement pour les chercheurs mais aussi pour les publics. Ces sites sont également devenu un moyen non négligeable pour rejoindre les publics et mais aussi participer à la construction d’une image de l’institution.

- comprendre comment elle s’inscrit dans des politiques institutionnelles plus générales (conernant le soutien à l’innovation technique, la transformation néolibérale, ou les politiques de données ouvertes)
- croiser les points de vue internationaux pour identifier des dynamiques distinctes selon les localités
- comprendre qu’il s’agit d’un terrain conflictuel qui présente de nombreux enjeux

#### Une question ethique plutôt que juridique

**Dès lors qu’ils étaient présents sur le web, les musées et les institutions patrimoniales se sont trouvé plongés dans une culture tout à fait nouvelle, celle de l’informatique.** L’augmentation de la bande passante a rapidement permis la diffusion d’images de plus grande qualité posant au même titre que pour la musique ou d’autres contenus diffusés sur le web la **question du réemploi et de la propriété intellectuelle**. Bien sûr, le secteur muséal ne présentait pas les mêmes enjeux commerciaux et industriel que celui de la musique ou du cinéma en termes de piratage, néanmoins rapidement émerge la problématique du réemploi de ces contenus et de leur utilisation libre par les internautes. Un phénomène qui s’est trouvé amplifié par le développement de contenus générés par les utilisateurs avec l’avènement des plateformes de blogs et les réseaux sociaux numériques.

**C’est dans ce contexte que la question des contenus muséaux et patrimoniaux est devenue une question militante et politique.** Plusieurs associations ont émergé (comme l’Open Knowledge Fondation, Savoirs Com1, COMMUNIA) pour défendre des communs numériques et ont été à l’origine de lia publication de différents manifestes pour revendiquer la publication des données de collections sous licences libres, mais aussi l’abandon des droits de reproduction et des restrictions appliquées par les institutions aux contenus culturels passés dans le domaine public. Ces groupes empruntent largement par leurs pratiques et leurs modes d’organisation à la culture et à l’éthique hacker qui s’était développée dans le domaine du développement logiciel et sur le web. 

De telles revendications rejoignirent plus largement des revendications sur la publication des données publiques (open data) et sur la transparence de l’action des gouvernements. **Si la distinction entre données et œuvres a d’abord servi de levier pour obtenir l’ouverture des données de catalogage, s’est rapidement posé la question des droits de reproduction des œuvres pour lesquels les musées se réservaient la perception de droits prohibitifs.** À travers la question juridique de la propriété des données ou de la titularisé du droit d’auteur, c’est en quelque sorte la mission et le rôle de l’institution muséale qui est interrogée. Le musée ne travaille-t-il pas pour le public ? À qui appartient les collections ? Dans quelle mesure, le musée peut-il revendiquer des droits sur les œuvres ? Ces différentes questions ont donné lieu à d’importants débats et une intense activité juridique qui témoigne du fait que le droit de la propriété intellectuel est encore un droit en évolution. Elle a aussi donné lieu à la publication de plusieurs manifestes et de guides de bonnes pratiques. Certaines institutions ouvrant la voie avec des pratiques exemplaires qui leur ont parfois permis de contribuer à leur rayonnement comme le Rijksmuseum, le MET, etc.

Si la question est renouvellée par le numérique qui facilite la copie des ressources sans perte, il s’agit en réalité d’une question posée de longue date au musée ainsi que le rappelle la déclaration ReACH pour la promotion universelle de la reproduction et du partage du patrimoine culturel à travers les technologies numériques en 2017. Cette initiative engagée par la national galery de Londres célébrait le 150e anniversaire de la convention d’Henry Cole de 1867, *Convention for promotion universelle reproductions of works of art for the benefit of museums of all countries*. 

The ReACH Declaration for Promoting Universally the Reproduction, Storage and Sharing of Works of Art and Cultural Heritage Through Digital Technology, 8 décembre 2017

>This declaration promotes **the vision that works of art and cultural heritage should be preserved and shared as widely as possible throughout the world**.
>
>Through advances in technology and connectivity, we now have **a revolutionary opportunity to enhance learning, creativity and innovation, and to reach new audiences worldwide**, through the reproduction and sharing of works of art and cultural heritage (‘Works’). Furthermore, digital technologies can enable us to record, document and, in some instances, recreate Works that are threatened by environmental hazards, conflicts, terrorism, rapid economic development, mass tourism, thefts and other natural and human-made disasters (‘Endangered Works’) or that have been lost.
>
>For cultural institutions that hold collections for the benefit of the public, the opportunity to provide open access now or in the future to Works in a digital format is **an exciting new frontier in their mission to preserve and transmit knowledge, culture and history for present and future generations**. Such opportunities also present responsibilities. Digital Records need to be responsibly created and safeguarded for the long term to ensure integrity as well as retrieval and reuse by future generations. Furthermore, as the means and skills required to use and access digital technology are not distributed evenly around the world, it is incumbent on those with the capacity to do so to provide support and training to those with fewer resources.
>
>This Declaration is intended for both institutions and individuals to promote the production, sharing and preservation of digital records and reproductions (‘Records’). Owners and Stewards of Works and others involved in the process of generating these Records are encouraged to disseminate and use the ReACH Declaration as widely as possible.

On n’envisage habituellement pas les musées comme des lieux destinés à la conservation de copies. Au contraire, l’institution muséale se définit plutôt en règle générale comme chargée de la conservation de choses vraies, d’artefacts du passés rassemblés dans des collections pour leur signification et leur valeur de témoignage. Pourtant, la convention de 1867 fut à l’origine d’une dynamique de création de musées de moulages qui ont joué une importance considérable dans la diffusion et la connaissance du patrimoine du passé.

La Reach déclaration appelle ainsi, à son tour, les musées à mieux s’engager sur la diffusion des reproductions par les moyens numériques, surtout à l’heure où ces technologies s’améliorent.

Restituer également la dynamique de revendication d’accès aux œuvres et de réappropriations.

- Les questions juridiques : open content / open data
- Notion de bien communs, ou de communs numériques

Situations diverses selon les continents et les pays. Revenir sur le cas Européen, le cas québécois.

Un mouvement social pour l’ouverture. Ouverture avant tout une question politique (souligner cas des politiques européennes)

- caractéristique militante et revendicatrice
- communautés d’amateurs
- enjeux sociaux de l’ouverture et réappropriation + enjeux éthiques

#### De riches pratiques numériques

comprendre comment, au-delà de l’injonction, certaines institutions à l’instar du Rijks par exemple, ont pu en faire un atout dans leurs politiques de médiation

Diversité des pratiques et des approches. Nouvelles modalités de diffusion

- avec les API, mais aussi un nouvel environnement logiciel
- projets collaboratifs Wikipédia
- nouveaux usages et culture du Remix



### La collection et le lieu

- Aura des objets, et chose vraie
- Identité des collections associées aux musées

Traditionnellement, le musée est défini par les collections qu’il conserve. 

Noter que définition actuellement en discussion. Unesco *Convention for the Safeguarding of the Intangible Cultural Heritage* (2006) et proposition de Ross Parry de reconnaître le collectionnement numérique, e-tangible (2007).

> Just as, a quarter of a century ago, museums grew formally to recognize ‘intangibles’ as valid material to collect and document, alongside their ‘tangibles’, so, in the past decade, museums have extended their conception of the collectable to accommodate also objects that are grasped through the intervention of a computer. These are museums’ new ‘e-tangibles’. (Parry 2007, p. 68)

Collection un ensemble d’unité discrètes qui participent toutes à son unicité et son originalité. Collection tout comme la provenance qui fournit un contexte aux œuvres qui les charge de signification.

Cependant la collection n’est pas un objet statique, elle dispose d’une historicité tant en ce qui concerne sa constitution que son déploiement qui participent tous deux à ses effets de sens.

Enjeux de la distribution libre et de leur réutilisation.

- dans quelle mesure reconfigure-elle la signification des collection ?
- qu’est-ce qui justifierait de considérer cette diffusion de manière distincte que la participation à une exposition ?
- quels nouveaux effets de sens dans un environnement numérique ?

### Le nouveau régime documentaire des collections

Réduction documentaire liée à la numérisation. Relations complexes entre l’original et la reproduction (Schweibenz)

Réintégration dans d’autres ensembles qui procède à une resémantisation des collections. Mais dorénavant déterritorialisées par rapport au musée. 

Démultiplication de l’œuvre qui peut être en même temps ici et dans un autre endroit.

Perte de contrôle de l’institution, lâcher prise. 

Émergence d’une multiplicité d’acteurs différents qui peuvent prendre contrôle sur les objets (communauté wikipédia, réseaux sociaux numériques, travaux de curations).

Valorisation reste néanmoins possible à travers cette libéralisation. Valeur d’usage, contribution à la notoriété des œuvres, rétro liens.

### Le rôle social des musées

Plus seulement montrer les objets. Muséologie numérique pas seulement présentation des objets en ligne sur le web. Part de plus en plus importante dans les missions des musées. Pervasivité de la collection numérique dans les actions de l’institution.

Envisager avec MacDonald le musée comme service d’information.

Souligner la question du rôle social.

Mais envisager le musée comme un service d’information, à l’instar des bibliothèques ou des centres de documentation.

= une redéfinition des missions des musées

= un nouveau genre d’institution, méta-collections ? 

ex. M+ museum 

> M+ is a new museum for visual culture in Hong Kong focusing on 20th and 21st century art, design, architecture and moving image. It will be a major component of the new West Kowloon Cultural District.
>
> In 2005, this mission statement was proposed for M+:‘... to focus on 20th and 21st century visual culture, broadly defined, from a Hong Kong perspective and with a global vision. With an open, flexible and forward-looking attitude, M+ aims to inspire, delight, educate and engage the public, to explore diversity and foster creativity.’
>
> Right from its inception therefore, M+ has aimed to develop content ‘from a Hong Kong perspective, the perspective of the “now”, and with a global vision’, from the “inside out”.
>
> https://mplus.org.hk/en/
>
> http://d3fveiluhe0xc2.cloudfront.net/media/_file/Building/The%20Competition_130418.pdf

### Manière dont la collection est envisagée à travers la focale du numérique

Paradigmes numérique et postdigital, lieux communs numériques

Numérique dans tout

- Partage
- Ouverture
- Décentralisation
- Collaboration
- Version

### Vers une nouvelle Conceptualisation des musées

Souligner la diversité et l’extrême richesses des pratiques mises en œuvre par les musées.

À bien des égards, on peut dire que la plateforme Europeana est caractéristique de la Convergence musée bibliothèque. Une convergence dont est directement issu l’acronyme GLAM pour Gallery, Libraries, Archives et Bibliothèque. Plusieurs publications envisagent à partir des années 90 cette convergence à l’instar de Corinne Welger Barboza avec son *devenir médiathèque du musée*. La culture open source des nouveaux médias signifie des interfaces ouvertes, la liberté de se connecter à des images techniques. D’une certaine manière même le code informatique constitue une sorte d’interface. On assiste donc à la multiplication des interfaces déployées par les musées pour la mise à disposition des données de leur collection. Parfois par l’intermédiaire d’Interface programmable (cad accessible à des client informatiques par voie programmatique) parfois sous la simple forme de Dump de données sur GitHub. Ces évolutions s’accompagnent parallèlement de l’apparition d’un nouvel environnement logiciel avec des protocoles tels que IIIF pour le partage d’images, la création d’APIs informatiques et surtout d’outils pour les consommer qui tirent parti des services ainsi constitués.

Avènement possible d’une nouvelle conceptualisation des musées

En 1991, dans un article intitulé *The museum as “information utility”*, George MacDonald et Stefen Alsford expliquent que traditionnellement les musées ont focalisé leur attention sur le passé (MacDonald et Alsford 1991). Leur préoccupation à l’égard des restes matériels du passé explique en partie leur focalisation sur les objets. Une orientation que reflète l’énumération des diverses définitions traditionnellement associées au musées : collectionnent, préservation, étude, exhibition, interprétation. Un ensemble d’activités qui se pratiquent généralement sur site. D’après les auteurs, cette «  focalisation introvertie  » a en quelque sorte convaincu les musées que leur raison d’être était leurs collections d’artefacts plutôt que de la considérer comme un outil à travers lequel nous apprenons à propos du passé. Ce qui explique aussi largement que les musées aient acquis l’image d’institutions caractérisées par les interdictions, archivant les reliques d’un passé mort, seulement accessible à une élite esthétique ou intellectuelle (MacDonald et Alsford 1991).

Dans cet article, qui paraît après-coup particulièrement visionnaire compte tenu des développements récents de la muséologie mondiale, les auteurs proposaient de ne plus seulement servir la collection, mais la société. Selon eux, l’évolution du contexte social et politique, tout autant que de celle des technologies justifiaient déjà que les institutions répondent mieux aux besoins informationnels de la société. Et de réclamer d’envisager le musée dans la perspective non pas strictement de ses fonctions, mais de ses produits.

- génération d’informations résultant d’activité de recherche
- perpétuation d’informations sur les collections
- l’organisation des relations entre des éléments discrets d’information, y compris la recontextualisation d’artefact
- la dissémination

**Cadre d’opération global**, théorie d‘opération unifiante reflétant le cycle de vie de l’information à travers l’ensemble des départements du musée.

**Rôle d’interface du musée entre le visiteur et l’objet identifié depuis longtemps** (édito Museum Management and Curatorship, 1990)

**Montrer que cette conception, même si elle est fondamentalement néolibérale dans son énonciation, rejoint très directement celle de l’imputabilité sociale des musées qui agite actuellement les institutions.**

Directeurs de grands musées interviewés sur l’avenir des musées au Canada en 2016 {Maguire 2016} Tous signalent l’engagement avec le public et rôle communautaire, la demande d’une autorité partagée. http://canadianart.ca/features/whats-the-future-of-canadas-museums/ Question de la démocratisation associée au fait de rendre le patrimoine numérisé accessible à tous. L’avènement des technologies a rendu le patrimoine de plus en plus pluraliste et moins dépendant des experts (Witcomb 2007)

La solution n’est donc non pas technique mais fondamentalement politique. Ce n’est pas un fait nouveau, et on sait tous combien le fait de disposer d’une image ne suffit pas à autoriser sa réutilisation. Mais au-delà des strictes questions d’autorité à laquelle permet notamment de répondre la mise à disposition d’interfaces programmables, pour les images la question fondamentale reste en grande partie politique. Que deviennent alors dans ce nouvel environnement logiciel les possibilités d’engagement avec les collections mais également que deviennent dans ce contexte les collections. Dès lors comment continuer à faire musée ? Où est le musée s’il est partout ou bien s’il devient distribué ?

- Quelles possibilités engagement avec collections.
- Que deviennent dans ce contexte les Collections ?
- Où peut-être le musée, s’il est partout ?

Avènement du musée imaginaire.

Dès lors comment continuer à faire musée ? **Où est le musée s’il est partout ou bien s’il devient distribué ?** Quelles éditorialisations possibles ?

Si l’on souhaite réellement voir ce genre d’interfaces se multiplier, il me semble impossible de seulement se focaliser sur la question des licences et des droits. On ne pourra pas faire l’économie d’une réflexion sur les conséquences pour les musées sur leur représentation et l’identité de leurs collections.

Il s’agit donc de comprendre ce qui peut accompagner cette évolution des musées comme service informationnel en faisant en sorte que ce modèle puisse s’aligner avec les valeurs portées par l’institution et le projet d’établissement.

Ne pas ignorer les risques de dissolution de l’identité des collections.

Prendre conscience des tensions en jeu dans les institutions pour faire avancer la belle promesse d’un accès riche et généralisés aux œuvres des collections qui est à portée de main. 



### Quelle approche ?

- histoire institutionnelle, généalogie
- observationnelle
- quid du juridique ? quid du technique ? quid du social ? = ensemble de domaine qui relève du culturel, politiques.

Construction d’un champ épistémique de l’ouverture qu’il convient de questionner

Formes des interfaces qui peuvent être envisagées de manière critique dès lors que conditionnent l’accès aux contenus. Ensemble qui s’inscrit dans un dispositif discursif par nature profondément politique.