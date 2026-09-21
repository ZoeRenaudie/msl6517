title: MSL6517-11
description: zoerenaudie, emchateau UdeM
theme: presentation/theme/remark-dark.css
name: inverse
layout: true
class: inverse

---

name: index
class: center middle

# Éthique des données

### MSL6517 – automne 2025 | Zoë Renaudie

.footnote[<https://studium.umontreal.ca/course/view.php?id=254809>]

???
ajout : Métadonnées et traçabilité : gestion de la preuveLa gestion des documents d'archives doit pouvoir s'appuyer sur des données cohérentes le long du cycle de vie des données. Il existe donc des normes de gestion des documents d'archives (ISO 15489), et une norme particulière sur les métadonnées (ISO 23081). 

---

## Le statut juridique des données culturelles

### Distinguer les niveaux

Il est crucial de différencier :

1. **L'œuvre elle-même** (l'objet physique ou son contenu intellectuel)
2. **La reproduction photographique de l'œuvre** (l'image numérique)
3. **Les métadonnées descriptives** (la notice documentaire)

Chacun peut être soumis à des régimes juridiques différents.

### Le droit d'auteur : critère d'originalité

Pour qu'une œuvre soit protégée par le droit d'auteur, elle doit être **originale**. Au Canada, la Cour suprême a défini deux critères dans l'arrêt CCH Canadienne Ltée c. Barreau du Haut-Canada (2004) :

- **Talent** : utilisation de connaissances personnelles, d'aptitudes acquises
- **Jugement** : discernement, formulation d'une opinion, évaluation de choix distincts

> « L'élément essentiel à la protection [...] est l'exercice du talent et du jugement. »

**Composantes du droit d'auteur** :
- **Droits patrimoniaux** : reproduction, distribution, communication au public (limités dans le temps : 70 ans en France et au Canada après la mort de l'auteur)
- **Droits moraux** : paternité, respect de l'intégrité (imprescriptibles et inaliénables)

**Le domaine public** : Passé le délai de protection, l'œuvre peut être utilisée librement.

### Le statut des notices documentaires

**Question** : Une notice d'œuvre est-elle protégée par le droit d'auteur ?

**Réponse générale** : **Non, dans la plupart des cas**, car les notices muséales :
- Contiennent des informations objectives et factuelles
- Sont rédigées selon des cahiers des charges normalisés
- Utilisent des vocabulaires contrôlés
- Laissent peu de place à l'expression personnelle

**Exception** : Si la notice contient des champs libres rédigés de manière créative (analyse iconographique détaillée, interprétation originale), ces parties pourraient être protégées.

**Conséquence pratique** : Pour faciliter le signalement et favoriser la réutilisation, les institutions culturelles publient de plus en plus leurs métadonnées sous **licences libres**.

### La protection des bases de données

En Europe (mais pas au Canada), il existe un **droit _sui generis_ sur les bases de données** (Directive UE 1996, transposée en France 1998). Ce droit protège l'investissement substantiel pour la production de la base (collecte, vérification, présentation). Durée : 15 ans, renouvelables.

Au Canada, pas de droit _sui generis_. Les bases peuvent être protégées par le droit d'auteur si elles remplissent le critère d'originalité (choix et arrangement), mais les faits eux-mêmes ne sont pas protégeables.

---

## Introduction

???


Le champ de l’informatique muséale n’est pas exempt d’enjeux éthiques que ce soit à l’égard des problématiques d’accès aux données que des mécanismes de production de ces données. Dans certains domaines, la production des données muséales peut présenter des enjeux éthiques importants, c’est bien évidemment le cas des données d’autorités dont on a vu qu’elle jouaient un rôle crucial dans l’écosystème du web de données mais c’est également le cas des collections autochtones.

#### Lectures

- [Hannah Turner. « The Computerization Of Material Culture Catalogues: Objects and Infrastructure in the Smithsonian Institution’s Department of Anthropology. » *Museum Anthropology*, vol. 39, n° 2, 2016.](http://onlinelibrary.wiley.com/doi/10.1111/muan.12122/full) DOI : 10.1111/muan.12122
- [« This Belongs to You » In *Sharing Is Caring: Openness and Sharing in the Cultural Heritage Sector ; [an Anthology\]*. Sanderhoff, Merete et Michael Peter Edson, dir., p. 20-126. Copenhagen: Statens Museum for Kunst, 2014.](http://www.smk.dk/en/about-smk/smks-publications/sharing-is-caring/)

---

layout: false

background-image: url(imagesMSL/museumAreNotNeutral.png)

???

> Les musées ne sont pas neutres. Ils ne sont pas séparés de leur  contexte social, des structures du pouvoir et des luttes de leurs  communautés. Et quand il semble qu’ils sont séparés, ce silence n’est  pas de la neutralité, c’est un choix – le mauvais choix.
>
> En tant qu’institutions hautement respectées dans nos sociétés,  les musées ont la responsabilité et le devoir de lutter contre  l’injustice raciale et le racisme anti-noir à tous les niveaux, depuis  les histoires qu’ils racontent jusqu’à la diversité de leur personnel.
>
> Derrière chaque musée, il y a des gens. Chacun d’entre nous doit  choisir de se tenir responsable de ses propres préjudices et de vérifier ses propres privilèges. Nous devons choisir de nous opposer au racisme  dans nos propres cercles et être prêts à apprendre à nous améliorer.”
>
> Extrait du communiqué de Lonnie G. Bunch, secrétaire de la Smithsonian Institution et co-président d’ICOM États-Unis (International Council of Museums).

---

## Les métadonnées ne sont pas neutres

- #### socialement construites
- #### un biais interprétatif
- #### multiplicité des points de vue et co-production du savoir

exemple .red[Reciprocal Research Network] https://www.rrncommunity.org

Travail de Susan Douglas (Univ. Guelph)

???

Les données ne sont pas neutres, elles sont socialement construites.

information systems as social and technical infrastructures

Elles peuvent dès lors manifester des biais interprétatifs.

Important de considérer la multiplicité des points de vue et la possibilité de co-cosntruction du savoir.

- Initiation aux croyances
- Apprendre des autochtones
- Appariellage critique, penser le discours autochtone en tant que connaissance. Discours source

> In the case of the Smithsonian's anthropology records, the normative naming strategies and methods of digitization can be “inverted” by conducting a full history of these systems. In doing so, we can come to understand the mundane and routine ways through which information is transferred and mediated in the medium upon which it is held. In the next section, I unpack a small portion of this history and explain how paper-based documentation systems were automated into the newly developed Smithsonian Institution computerized system in the late 1960s. How information was transferred to the digital system elucidates a practice that was based in a specific epistemological moment regarding what ethnographic collections should be and how they should “correctly” be recorded so as to be useful for ethnographic research.
>
> http://onlinelibrary.wiley.com/doi/10.1111/muan.12122/full

Clavir M. L’intégrité conceptuelle de la conservation dans les musées, Muse, vol. 12, n° 3, p. 35-39.

Ames MM, 1986 Indians as resources : The changing relationship Between Indians and Anthropologists, Wicazo Sa Review, vol. 2, n° 1, p. 10-13.

Clifford J 1996 [1988] Malaise dans la culture, L’ethnographie, la littérature et l’art au XXe siècle, Paris, École nationale supérieure des Beaux-arts.

Dubuc É et Turgeon L. 2004, Musées et Premières Nations, Anthropologie et sociétés, vol. 28, n° 2.

---

background-image: url(imagesMSL/rijksmuseumServiteurNoir.jpg)

.footnote[« Le serviteur n » (tableau de Jan Mijtens, 1668) a été rebaptisé « Jeune serviteur noir ». Rijksmuseum]

???

Bosc-Tiessé, Claire. 2019. « Le cartel des arts. Enjeux d’histoire entre assignations ethnographiques et présentations muséales ». *Afriques. Débats, méthodes et terrains d’histoire*, no 10 (décembre). https://doi.org/10.4000/afriques.2651.

Cartels

> Ce projet baptisé « Ajustements au sujet des terminologies colonialistes » comme le reporte le site [Exponaute](http://www.exponaute.com/magazine/2015/12/14/le-rijksmuseum-ote-de-ses-titres-et-encarts-des-termes-racistes-et-sexistes/) aurait pour objectif de « ne pas offenser les visiteurs étrangers ». 8.000 titres d’œuvres auraient déjà été modifiés. Le site prend comme exemple le surnom que portaient les Hollandais : « têtes de fromage » (« kaas kops » en néerlandais) – car on le sait bien les fromages hollandais sont très célèbres. Gosselink explique lors de la conférence de presse que des Hollandais en visite dans un musée étranger n’apprécieraient guère de tomber sur un titre d’oeuvre comme « Femme tête de fromage ». Rappelons tout de même qu’il existe des titres bien plus violents que ceux qui font appellent à des plaisanteries fromagesques notamment pour les représentations de personnes racisées.

## Environ 220.000 descriptions concernées 

Jeudi 10 décembre 2015, Martine Gosselink, chargée du département d’Histoire du Rijksmuseum Amsterdam, a présenté son projet lors d’une conférence de presse : enlever des titres et cartels tout terme réducteur ou discriminant issu de l’eurocentrisme et de la suprématie impérialiste du continent. 220.000 œuvres sont ainsi concernées.

*« mahométan »*, *« maure », « nain »* ou encore *« sauvage »*, 23 termes jugés offenssants, racistes, sexistes ou discriminatoires

A ce jour, 8.000 descriptions environ ont été changées. Au final, les modifications de titres vont concerner quelques 220.000 panneaux. Par exemple, le tableau de Simon Maris (photo à la Une), intitulé « Jeune femme n**** » a été rebaptisé « Jeune fille à l’éventail ». Le titre n’avait pas été choisi par le peintre, mais par un collectionneur.  

Parmi eux, entre autres, *La Toilette de Bethsabée*, de Cornelis van Haarlem, peinte en 1594. Aujourd'hui, sur le site du Rijksmuseum, la description du tableau indique : *« Parce que la servante de Bethsabée est noire, cette peinture subtilement érotique se pare d'une touche d'exotisme. »* Le musée confirme au *Monde* que cette phrase devrait disparaître. 

Le Rijksmuseum précise avoir pris cette mesure après de nombreuses plaintes de visiteurs, jugeant les titres de certaines œuvres racistes ou sexistes. Et l’institution se défend de céder à une quelconque idéologie du « politiquement correct ». 

Pour Martine Gosselink, directrice du département d'histoire du musée et responsable du projet, « *autrefois, nous avions des mots offensants pour tout le monde. Les Africains, les Japonais, les Allemands... Nous nous sommes dit qu'en 2015, on ne s'adressait plus les uns aux autres sur ce ton-là* ». « *Rien qu'aux Pays-Bas, il y a un million de personnes issues des anciennes colonies ; du Surinam, des Antilles, d'Indonésie. Ne serait-ce que pour cette raison, il est important de procéder à ces modifications*», a-t-elle ajouté. 

Supprimer histoire ?

Et d'assurer que tous les titres seront gardés, dans la base de données  du musée s'ils ont été choisis par les collectionneurs, et en dessous du nouveau titre, à disposition des visiteurs, s'ils ont été choisis par  l'artiste.

Alternative : valoriser cartel longs

Exemple Musée d’Aquitaine, exposition permanente Bordeaux au XVIIIe siècle, le commercie atlantique et L’esclavage. 2019

*Le Monde.fr*. 2019. « Le Musée d’Aquitaine affiche un cartel aux relents révisionnistes sur la traite négrière », 21 mai 2019. https://www.lemonde.fr/idees/article/2019/05/21/le-musee-d-aquitaine-affiche-un-cartel-aux-relents-revisionnistes-sur-la-traite-negriere_5464839_3232.html.

>Selon le collectif d’écrivains à l’origine de la tribune parue dans Le Monde, un des textes de l’exposition relèverait de la *« tartufferie langagière »*. Le lexique du musée pour dépeindre les circonstances du trafic d’esclaves à Bordeaux ne correspondrait pas à la réalité des faits.
>
>Les signataires pointent ainsi du doigt un usage inadapté du mot *« formation »* concernant le travail des débarqués. Ailleurs, s’agissant de la capture et du transport des esclaves vers la France, ils épinglent la phrase « Noirs et gens de couleurs viennent à Bordeaux au XVIIIe siècle ». *« De leur propre chef ? Par goût du voyage ? »*, ironisent-ils.
>
>Alors que les auteurs de la tribune dénoncent une *« désinformation insidieuse aux relents révisionnistes »*, [Laurent Védrine](https://www.lejournaldesarts.fr/personnalite/laurent-vedrine-2030), directeur du Musée d’Aquitaine, s’est dit *« choqué »* auprès du *Journal des Arts* de la « violence des termes » visant un cartel *« décontextualisé, alors même que l’exposition dans laquelle il s’inscrit est entièrement consacrée à la mémoire de la traite négrière bordelaise. »**
>
>**« Je conçois que les mots choquent »*, reconnaît cependant Laurent Védrine tout en rappelant que, l’an dernier, en réponse à une lettre rédigée en ce sens par l’une des signataires de la tribune, il avait indiqué être conscient du problème, et affirmé qu’un renouvellement des cartels était prévu.
>
>*« Le texte dont il est question est là depuis 10 ans, et n’avait jusqu’alors jamais posé problème. Il faisait néanmoins partie des cartels que nous comptions modifier. Mais réorganiser une muséographie sur des sujets aussi sensibles demande du temps »*, s’est défendu le directeur du musée bordelais pour se justifier. 
>
>Face à l’escalade de la controverse, le Musée d’Aquitaine a bousculé son agenda. Le cartel a été remplacé en début de semaine. 
>
>https://www.lejournaldesarts.fr/patrimoine/critique-le-musee-daquitaine-retire-un-cartel-144377

---

background-image: url(imagesMSL/rijksColonialPast.png)

???

Volonté des musées, à l’instar du Rijksmuseum de reconsidérer leurs récits en s’adressant à une nouvelle clientèle.

---

template: inverse

class: center middle

## Les enjeux éthiques liés à la production des données

---

layout: false

## Code de déontologie de l’ICOM pour les Musées

1. Les musées assurent la protection, la documentation et la promotion du patrimoine naturel et culturel de l’humanité
2. Les musées qui détiennent les collections les conservent dans l’intérêt de la société et de son développement
3. Les musées détiennent des témoignages de premier ordre pour constituer et approfondir la connaissance
4. Les musées contribuent à la connaissance et à la compréhension et à la gestion du patrimoine naturel et culturel
5. Les ressources des musées offrent des possibilités d’autres services et avantages publics
6. **Les musées travaillent en étroite coopération avec les communautés d’où proviennent les collections, ainsi qu’avec les communautés qu’ils servent**
7. Les musées opèrent dans la légalité
8. les musées opèrent de manière professionnelle

ICOM. Code de déontologie de l’ICOM pour les Musées. 2017. ISBN 978-92-9012-421-4 http://icom.museum/fileadmin/user_upload/pdf/Codes/ICOM-code-Fr-web.pdf

???

ICOM. Code de déontologie de l’ICOM pour les Musées. 2017. ISBN 978-92-9012-421-4 http://icom.museum/fileadmin/user_upload/pdf/Codes/ICOM-code-Fr-web.pdf

> Les questions relatives à l’éthique dans le monde des musées, aux niveaux national et international, ont pris de l’importance au cours de ces dernières années. dans le monde entier l’intérêt pour des sujets liés à l’impact de la colonisation sur des populations soumises, les collections établies au cours de l’histoire par l’expansion d’empires, les demandes de restitution de peuples indigènes, le pillage d’art, l’art en tant que trophée et le trafic illicite (résultant parfois de conflits armés) s’est considérablement accru.
>
> http://icom.museum/fileadmin/user_upload/pdf/Codes/110831_Checklist_FR.pdf

Code déontologie, normes minimales en termes de pratiques professionnelles. Accent sur les missions de l’instituions et son rôle et son positionnement à l’égard des communautés qu’elle sert ou dont sont issues ses collections.

Le Code d’éthique professionnelle de l’ICOM a été adopté unanimement au cours de la quinzième assemblée générale de l’ICOM à Buenos Aires (Argentine) le 4 novembre 1986. Celui-ci fut amendé lors de la vingtième assemblée générale de Barcelone (Espagne) le 6 juillet 2001, et réintitulée ICOM Code of Ethics for Museums, et révisée au cours de la vingt-et-une-nième assemblée générale à Séoul (République de Corée) le 8 octobre 2004.

1. Les musées assurent la protection, la documentation et la promotion du patrimoine naturel et culturel de l’humanité
2. Les musées qui détiennent les collections les conservent dans l’intérêt de la société et de son développement
3. Les musées détiennent des témoignages de premier ordre pour constituer et approfondir la connaissance
4. Les musées contribuent à la connaissance et à la compréhension et à la gestion du patrimoine naturel et culturel
5. Les ressources des musées offrent des possibilités d’autres services et avantages publics
6. Les musées travaillent en étroite coopération avec les communautés d’où proviennent les collections, ainsi qu’avec les communautés qu’ils servent
7. Les musées opèrent dans la légalité
8. les musées opèrent de manière professionnelle

Souligner le rôle déterminant des institutions muséales dans la documentation, la connaissance et la promotion du patrimoine. Institutions fiduciaires qui doivent agir dans l’intérêt de la société et de son développement. Ce qui implique notamment de servir les communautés mais aussi d’agir et de travailler en étroite coopération avec les communautés qu’ils servent mais aussi d’où peuvent provenir les collections.

Titre de propriété, provenance et obligation de diligence.

Témoignage de premier ordre 

- type de discours mobilisé
- disponibilité des collections et des informations les concernant

Collecte et recherche par le musées

- conforme aux normes scientifiques
- mais aussi "avec respect et considération pour les points de vue des communautés locales, de leurs ressources environnementales et de leurs pratiques culturelles, ainsi qu’en tenant compte des efforts déployés pour mettre en valeur le patrimoine culturel et naturel." (Code déontologie, p. 19)

Présentation et exposition

- "4.2 Interprétation des éléments exposés
  Les musées doivent veiller à ce que les informations qu’ils présentent dans leurs expositions soient fondées, exactes et prennent en considération les croyances et groupes représentés." (Code déontologie, p. 25)
- cf. exposition de restes humains et objets "sensibles", mais aussi demandes de retours des objets cultuels

Coopération avec les communautés

- coopération avec les communautés d’origine
- retours et restitution des biens culturels

> Respect des Communautés servies
>
> 6.5 Communautés existantes
> Si les activités du musée mettent en jeu une communauté existante, ou son patrimoine, les acquisitions ne doivent s’effectuer que sur la base d’un **accord éclairé et mutuel**, sans exploitation du propriétaire ni des informateurs.
> Le respect  des vœux de la communauté concernée doit prévaloir.
>
> 6.6 Financement des a ivités et communautés
> La recherche d’un finnancement pour des activités muséales impliquant une communauté existante ne doit pas nuire aux intérêts de cette communauté (voir aussi 1.10).
>
> 6.7 Utilisation de collections de communautés existantes
> L’utilisation de collections provenant de communautés existantes doit respecter les principes de dignité humaine ainsi que les traditions et les cultures de la communauté d’origine. Ce type de collections doit être utilisé pour promouvoir le bien-être, le développement social, la tolérance et le respect en favorisant l’expression multisociale, multiculturelle et multilinguistique (voir aussi 4.3).
>
> 6.8 Organisations de soutien
> Les musées doivent créer des conditions propices à un soutien communautaire (par exemple avec les associations d’Amis de musées et autres organisations de soutien), prendre acte de cet apport et promouvoir des relations harmonieuses entre la communauté et le personnel de musée.
>
> (Code de déontologie, p. 34)

---

background-image: url(imagesMSL/mcn2016-the-future-of-museum-technology.png)

???

les musées et la justice sociale, l’exemple de **Black lives matter**

---

background-image: url(imagesMSL/spiritsings.jpg)

.footnote[Catalogue d’exposition et vue de l’exposition, *The Spirit Sings : Artistic Traditions of Canada's First Peoples*, Glenbow Museum, 1er juillet au 6 novembre 1988.]

???

inclure les diverses composantes ethniques ou minoritaires

Dubuc 2004 : instauration d’une muséologie collaborative au musée d’anthropologie de l’Université de la Colombie-Britannique en établissant un mode de fonctionnement ouvert aux communautés autochtones.

Depuis la fin des années 80, les collaborations avec les communautés autochtones se sont accrues dan les musées canadien. Après la remis en cause des musées ethnologiques, reconnaissance de la parole autochtone.

- redonner dignité et respect aux populations
- produire des expositions qui présentent leur patrimoine d’origine en tenant compte de leur point de vue

Polyphonie de reconnaissance

Problèmes suscité par le patrimoine autochtone dans les musées, soit parce qu’il a été collecté durant la colonisation soit parce que les communautés revendiquent leur patrimoine et un droit de parole.

Manifestations contre l’exposition *The spirit sings: artistic traditions of Canada’s first people* du musée Glenbow à Calgary, pendant les jeux olympiques d’hiver 1988.

---

background-image: url(imagesMSL/RebeccaBelmore.jpg)

.footnote[Rebecca Belmore, *Artifact #671B,* 1988, performance, Thunder Bay, Ontario.]

???

Shell Canada mécène de l’exposition alors que s’appropriait les territoires autochtones. 

Action à l’appel de la Première Nation du Lac Lubicon. Boycottage qui a notamment conduit à l’organisation de plusieurs rencontres nationales entre les peuples autochtones et les musées.

Posaient la question de savoir le genre de rôle que les autochtones devaient jouer dans la mise en valeur de leur propre passé, de leur propre histoire ?

---

background-image: url(imagesMSL/tournerLaPage.jpg)

.footnote[*Rapport du Groupe de travail sur les musées et les Premières Nations – Tourner la page : forger de nouveaux partenariats entre les musées et les Premières Nations* publié en 1992 par l’Assemblée des Premières Nations et l’Association des Musées Canadiens. http://museums.in1touch.org/uploaded/web/docs_fr/Task_Force_Report_1994_FR.pdf]

???

Quand l’exposition est venue à Ottawa, l’Assemblée des Premières Nations a considéré ce qu’elle pouvait faire. Au lieu de continuer le boycott, celle-ci a préférer essayer de le dépasser en engageant le début d’un nouveau type de relation "entre deux grands alliés potentiels." (Georges Erasmus, ancien chef national de l’Assemblée des Premières Nations)

Georges Erasmus a invité George MacDonald, directeur du Musée canadien des civilisations à coparrainer un colloque traitant des points controversés entre les musées et les Premières Nations. Lors de cette rencontre, il fut décider de mettre sur pied un groupe de travail destiné à "développer un système et des stratégies éthiques permettant aux peuples autochtones et aux institutions culturelles de travailler ensemble pour représenter l’histoire et la culture autochtones." (Rapport, 1)

*Rapport du Groupe de travail sur les musées et les Premières Nations – Tourner la page : forger de nouveaux partenariats entre les musées et les Premières Nations* publié en 1992 par l’Assemblée des Premières Nations et l’Association des Musées Canadiens.

Résultat de la contribution de nombreuses communautés et discussion ouverte sur tout le territoire.

http://museums.in1touch.org/uploaded/web/docs_fr/Task_Force_Report_1994_FR.pdf

**Intention : "Développer un cadre de travail et des stratégies éthiques qui permettront aux Nations aborigènes de représenter leur histoire et leur culture de concert avec les institutions."**

Encourage le partenariat et la participation active des autochtones dans les musées :

- **Reconnaissance de l’importance des objets culturels** dans les collections de musées, représentation des valeurs culturels, sources d’apprentissage, de fierté et d’amour propre. Pour soi et plus généralement.

- **Implication accrue des Premières Nations dans l’interprétation**. Interprétation qui inclut toutes les facettes de l’administration, de la recherche, de la programmation et de la planification des expositions par les musées, ainsi que les présentations qui en résultent. = recommande l’élargissement de l’implication des autochtones dans l’interprétation des collections et la mise en valeur des cultures vivantes
- **Accès amélioré aux collections de musées** (y compris matériel pour utilisation cérémoniale) et rapatriement = conditions de rapatriement, de conservation et de présentation des objets

Actions :

- réclame inventaire "aussitôt que possible et mis à la disposition des communautés autochtones appropriées"
- Formation et soutien aux institutions

Principes de création de nouveaux partenariats

- Présentation comme cultures mortes ou en voie d’extinction (présentation renforçant conception voulant que les cultures aborigènes n’aient existé que dan le passé et qu’elles seraient incapables de changer. = alimente notion erronée selon laquelle les cultures aborigènes seraient inférieures)
- Reconnaissance contribution unique fondamentale des Premières Nations

Droit à parler pour elles mêmes

partenariat égal, connaissances mutuelles

intérêt mutuel

cogestion et coresponsabilité

Implication

Pour l’interprétation :

- particiaption
- éthique de responsabilité et professionelle
- travail en collaboration, utilisation langue autochtones pour identification du matériel

L’implication des autochtones au sein des musées laisse entrevoir de meilleure forme d’exposition. Ce modèle d’exposition, qualifié en anglais de « *multivocal* », est traduit en français par le néologisme « plurivocalité » (Dubuc et Turgeon, 2004, p. 11).

cf. Virginie Soulié https://www.erudit.org/en/journals/ef/2015-v43-n1-ef01833/1030183ar.pdf

---

- Recommandations du protocole de recherche de l’Assemblée des Premières Nations du Québec et du Labrador (APNQL) adopté en juin 2005. http://www.cssspnql.com/docs/centre-de-documentation/protocole-de-recherche---synthese.pdf?sfvrsn=2
- Musées de la Civilisation, Québec. Politique des Musées de la civilisation à l’égard des peuples autochtones, 27 septembre 2012 https://www.mcq.org/documents/10706/21548/pltq_autochtone__anx_fr_vf_maj_20150204.pdf/84dc0e01-2526-4347-929c-341e068f9135
- Musée des beaux-arts du Canada, plan stratégique 2021-2026 https://www.beaux-arts.ca/a-propos/plan-strategique
- Association des musées canadiens. Portés à l’action : Appliquer la DNUDPA dans les musées canadiens, En réponse à l’appel à l’action n° 67 du rapport de la Commission vérité et réconciliation, 2022 https://museums.ca/uploaded/web/TRC_2022/Rapport-AMC-Portesalaction.pdf

???

### Décoloniser les pratiques muséales

Volonté de "décoloniser" les pratiques muséales, en tenant compte du point de vue autochtone.

Autorité de l’ethnologie : Jamin 1998, Faut-il brûler les musées d’ethnographie. Fisher, Marcus, Clifford, et Fabian.

- pratiques entachées du modèle colonial
- transformation de l’anthropologie également associée au colonialisme.

Ames dit qu’en tant que professionnel de musée doit se détacher du champ théorique de l’anthropologie. Ce qui signifie également se départir de son arsenal scientifique et de sa fonction critique. (Ames 1986, 1987, 1992, 1999)

Construction de modèles pluri vocaux (Dubuc et Turgeon 2004)

Clifford 1988 qui a notamment mis en évidence plusieurs enjeux documentaires en retraçant l’histoire de la logique taxinomique des objets ethnologiques et en identifiants les différents statuts conférés aux objets "extra-occidentaux".

Critique les logiques culturelles et artistiques de la documentation de ces objets, en soulignant notamment la part de subjectivité de ces statuts. 

Suggère la valorisation et la prise en compte du point de vue des peuples autochtones, pour constituer d’autres statuts et attribuer de nouvelles interprétations aux objets (Virginie Soulier 2013 : 30).

ex : séparation entre le spirituel et le culturel, rapport aux objets rituels

Nécessaire ajustement en conséquence des pratiques de conservation. Équilibre entre les besoins et les usages des propriétés culturelles et la conservations des propriétés culturelles. Intégrité conceptuelle vs intégrité matérielle (Clavir 1994)

http://www.archipel.uqam.ca/8088/1/D2626.pdf

### Exemple des Musées de la civilisation Québec

Rôle important de la diffusion, notamment numérique.

Caractère prioritaire de la diffusion des informations se rattachant à ces collections.

> Afin de donner un cadre éthique à leurs projets, notamment en ce qui a trait à la collecte d’informations qualitatives et quantitatives, les Musées de la civilisation s’inspirent des recommandations du protocole de recherche de l’Assemblée des Premières Nations du Québec et du Labrador (APNQL) adopté en juin 2005.
>
> Propriété, Conrtôle, Accès, Possession.
>
> PROPRIÉTÉ — Principe lié à la détention personnelle et collective des informations.
> Les données et autres informations récoltées doivent être retournées dans les communautés, villages et institutions autochtones qui ont participé à la recherche, ainsi qu’aux individus ayant participé à cette recherche.
>
> CONTRÔLE — Principe qui souligne la nécessaire participation des membres des Premières Nations à toutes les étapes du processus de recherche.
> Informer clairement les participants à la recherche et leur permettre de réorienter, si nécessaire, les objectifs de la recherche;
> Travailler en étroite collaboration avec un comité scientifique (composé de chercheurs issus du milieu académique) et un comité culturel (composé de personnes ressources et d’experts issus des communautés, villages ou organisations autochtones).
>
> ACCÈS — Principe qui exprime le droit de regard sur l’information et les données.
> Favoriser le partage de toutes les données ou informations ayant été archivées aux Musées de la
> civilisation.
>
> POSSESSION — Principe qui renvoie à l’affirmation et à la protection du principe de propriété.
> Formaliser la collaboration par le biais d’ententes précisant les rôles et les responsabilités de chacun des partenaires, et de formulaires de consentement individuel.

> L’élaboration de ce protocole ne vise certes pas l’entrave d’investigations critiques ou toute forme de travaux susceptibles d’aboutir à des conclusions indésirables, mais plutôt de promouvoir une recherche éthique précise et bien informée, dont le déroulement respecte la volonté des Premières Nations impliquées. (Avant-propos du Chef Ghislain Picard)

### Musée des beaux-arts du Canada

2022, le musées des beaux-arts du Canada crée un nouveau département des voix autochtones et décolonisation

Steven Loft VP et Michelle LaVallee dirctrice du département.

2021, le mot *Ankosé*. Notre nouvelle [raison d'être institutionnelle](https://www.beaux-arts.ca/a-propos/enonce-de-mission) – *favoriser les interrelations dans le temps et l’espace* – nous invite à mener des conversations difficiles, à voir le monde selon des points de vue différents et à inspirer l’empathie et l’humilité. Tel est le socle du nouveau plan stratégique du Musée, [*Transformer ensemble*](https://www.beaux-arts.ca/a-propos/plan-strategique)*.*

https://www.beaux-arts.ca/collection/a-propos-des-collections/voies-autochtones-et-decolonisation#:~:text=La%20collection%20d%27art%20autochtone,de%20l%27art%20en%20Occident.

https://www.beaux-arts.ca/pour-les-professionnels/medias/communiques/le-musee-des-beaux-arts-du-canada-cree-un-nouveau

https://www.beaux-arts.ca/a-propos/lhistoire-de-notre-marque

---

## Déclaration des nations unies sur les droits des peuples autochtones

« Déclaration des nations unies sur les droits des peuples autochtones (DNUDPA) ». UNESCO, 2007. https://fr.unesco.org/indigenous-peoples/undrip.

Appel à l’action n° 67 de la Commission de vérité et réconciliation (2015)

> Nous demandons au gouvernement fédéréal de fournri des fonds à l’Association des musées canadiens pour entreprendre, en collaboration avec les peuples autochtones, un examen national des politiques et des pratiques exemplaires des msuées, et ce, dans le but de déterminer le degré de conformité avec la Déclaration des Nations Uniers sur les droits des peuples autochtones et de formuler des recommandations connexes.

Danyluk, Stephanie, et Rebecca MacKenzie. « Portés à l’action : Appliquer la DNUDPA dans les musées canadiens ». Association des musées canadiens, 2022. https://www.museums.ca/site/movedtoaction?language=fr_FR&.

---

background-image: url(imagesMSL/premieresNations.jpg)

.footnote[Affiche de l’exposition Premières Nations, collections royales de France, Musée de Pointe-à-Caillière, 5 juin 2007-14 octobre 2007]

???

Dans sa thèse de doctorat, Virginie Soulier cite l’exemple d’une exposition temporaire des collections du Quai Branly au Musée de Pointe-à-Caillère qui a fait l’objet d’un ajustement dans un souci de représentativité.

Premières Nations, collections royales de France, du 5 juin 2007 au 14 octobre 2007

Cette exposition a été conçue et présentée au musée du quai Branly à Paris, sous la responsabilité scientifique de M. Christian Feest, commissaire de l’exposition.

15e anniversaire de Pointe-à-Caillière, 85 objets choisis parmi les plus beaux des collections amérindiennes du musée du quai Branly à Paris.

> Il s’agit de **l’une des plus riches collections au monde d’objets amérindiens** des 18e et 19e siècles provenant de l’Est de l’Amérique du Nord. Appartenant à l’origine aux collections des rois et des aristocrates de France, ces objets reflètent l’intérêt qu’a porté la France coloniale à la Nouvelle-France.
>
> https://pacmusee.qc.ca/fr/expositions/detail/premieres-nations-collections-royales-de-france/

Précautions mises en place par le musée sur la production de l’exposition, modification de l’exposition intinérante.

Critique de Price à l’égard du musée du Quai Branly.

Point sur l’exposition prêtée et la documentation des objets afin d’établir ses propres orientations.

Quels sont les objets autochtones de l’exposition : 85 objets sur 87, datant du XVIIe au XIXe siècle, la plupart datant de la seconde moitié du XVIIIe siècle. Ces objets provenaient de 19 nations autochtones différentes, la majorité iroquoises et huronnes.

Diversité de l’origine des objets, mais prédominance des territoires de l’Est liée à l’histoire coloniale française.

Contexte de collectionnement, cabinets de curiosité. Échanges, troc mais aussi spoliation. Travail de documentation sur la provenance et transferts successifs.

Notamment Collection du Cabinet du roi, déplacée à la BnF, puis 1878 au Musée d’ethnographie du Trocadéro devenue Musée de l’homme en 1937.

La plupart d’origine royale vérifiée.

Cheminement interprétatif méritant d’être expliqué, comme représentatif de l’histoire des collections autochtones ou plus exactement de l’intérêt français à l’égard de ces collections.

Question de la dénomination de ces objets qui a changé au cours du temps. Comment se situer par rapport à l’héritage français et autochtone.

Poche, sac à tabac, or le plus souvent des sacs à feu pour transporter le matériel servant à faire du feu, ou bien des sacs à plomb pour la chasse.

Robe, notion utilisée dès le XVIIIe siècle, objets qualifiés de "manteaux ou tabliers des Illinois" ce qui est plus conforme à la manière de les porter à cette époque (en cape sans capuchon). Choix des termes.

Meilleure connaissance des objets d’usage, mais se rend compte des difficultés pour interpréter et nommer les collections.

—> cherche à établir des règles constantes et cohérentes dans la manière de décrire les objets, et rendre compte des différents points de vue.

Classification des objets. Dans le catalogue, trois catégories qui constituent les zones thématiques principales de l’exposition.

- vêtements et ornements, première catégorie centrée sur la fonctionnalité des objets
- vie sociale, la guerre et la paix : en tant que représentant d’une certaine "vision du monde", y inclut la religion
- arts de la maison : rend compte des techniques et des matériaux de fabrication

> En utilisant et en adaptant la nomenclature de Cehnhall (1978, 1995), on peut classifier autrement les objets. Cette méthode a pour avantage de classifier les objets à partir de leur fonctionnalité première de manière plus constante et précise. Cet exercice permet de prendre du recul à l’égard de l'interprétation faite par le commissaire pour repenser la typologie différemment. Trois catégories sont ainsi construites : 1. objets usuels, outils et équipements, 2. objets personnels, parures et couvre-chefs, 3. objets cérémoniels, communication et symboles.
>
> (Virginie Soulier, 178)

Adaptation de l’exposition, contexte sensible du canada, où descendants présents. Intérêts différents du public et potentiel communicationnel des objets.

Scénario autour de trois lignes conceptuelles "1 la rencontre, 2 la découverte mutuelle avec ses partages échanges et affrontement, 3 l’entretien et l’approfondissement des liens tissés."

paix sociale, alliance.

Comité qui soulève problème causé par la thématique de l’échange car la plupart des objets des objets usuels sans rapport avec les français.

Objets sensibles, recommandations pour leur mise en exposition. Révision de l’identification des objets. Question de la traduction, ou de la langue, toponymes etc.

---

background-image: url(imagesMSL/rrn.png)

## Reciprocal Research Network (RRN)

https://www.rrncommunity.org

???

Reciprocal Research Network (RRN) is an innovative partnership between the Musqueam Indian Band, the Sto:lo Nation and Sto:lo Tribal Council, the U’mista Cultural Society, and the University of British Columbia’s Museum of Anthropology, which was developed ‘to facilitate reciprocal and collaborative research’.5

Dyson L, Henriks M and Grant S (2007) Information Technologies and Indigenous Peoples. Hershey, PA: Information Science Publishing.

Gillespie T (2007) Wired Shut: Copyright and the Shape of Digital Culture. Cambridge, MA: MIT Press. Graber C and Burri-Nenova M (eds) (2008) Intellectual Property and Traditional Cultural Expressions in a Digital Environment. Cheltenham: Edward Elgar.

Johnson V (1996) Copyrites: Aboriginal Art in the Age of Reproductive Technologies. (touring exhibition catalogue). Sydney: National Indigenous Arts Advocacy Association and Macquarie University.

---

## National Indigenous Knowledge and Language Alliance

https://www.nikla-ancla.com

First Nations, Métis, and Inuit – Indigenous Ontology (FNMIIO).

https://nationalindigenousknowledgeandlanguagealliance.home.blog/2019/06/21/first-nations-metis-and-inuit-indigenous-ontologies-fnmiio/

>Decolonize Access and Classification by addressing the structural biases in existing schemes of knowledge organization and information retrieval arising from colonialism by committing to integrating Indigenous epistemologies into cataloguing praxis and knowledge management.
>
>CFLA-FCAB Truth & Reconciliation Committee report

???

Stacy Allison-Cassin, York University bibliothécaire LOD. A travaillé sur LCSH sujets indigènes, décolonisation des bibliothèques.

https://sacassin.blog.yorku.ca

https://nationalindigenousknowledgeandlanguagealliance.home.blog/2019/06/21/first-nations-metis-and-inuit-indigenous-ontologies-fnmiio/

---

background-image: url(imagesMSL/OPNMI.png)

.footnote[L’[Ontologie des Premières Nations, des Métis et des Inuits (OPNMI)](https://docs.google.com/spreadsheets/d/e/2PACX-1vSOKcm9HB-28iSqNN3sQd5hV7bMLMGpCeGL0dkQgyg2AiZAMWUF0sp98GyxIvLXYIWqSZ3nX_j_q4UN/pubhtml) publiée par l’Alliance nationale des connaissances et langues autochtones (ANCLA)]

???

Commission vérité et réconciliation 2008

> Ainsi, en 2016, le projet conjoint de [Wikimedia](https://www.wikimedia.org/) avec l’[Association of Research Libraries (ARL)](https://www.arl.org/) et les Autochtones d’Amérique du Nord, figure parmi l’une des réponses  aux appels à l’action pour la promotion et le développement de leur  culture et de leurs langues.

*Advancing Reconciliation and Social Justice in Libraries  through Research Library and Community Collaboration in Wikimedia  Projects*

[Stacy Allison-Cassin](https://sacassin.blog.yorku.ca/), l’appellation offensive « Indiens d’Amérique du Nord » plutôt qu’« Autochtones 

> Both Indigenous and non-Indigenous library and information science (LIS) professionals have long criticized the Eurocentric bias of these  systems: Indigenous names for peoples and places are either not used or  inaccurately Anglicized; Indigenous sovereignty and worldviews are  unrecognized; almost all literature save some aspects of tribal law are  classed narrowly in American history regardless of their currency; and  ideologically-biased terminology renders invisible the genocides  committed by colonial states against Indigenous North Americans.

> https://medium.com/museonum/se-raconter-avec-ses-propres-mots-la-d%C3%A9colonisation-du-patrimoine-indig%C3%A8ne-dans-les-96bc39de4e02

https://www.wikidata.org/wiki/Wikidata:WikiProject_Indigenous_peoples_of_North_America

> L’[Ontologie des Premières Nations, des Métis et des Inuits (OPNMI)](https://docs.google.com/spreadsheets/d/e/2PACX-1vSOKcm9HB-28iSqNN3sQd5hV7bMLMGpCeGL0dkQgyg2AiZAMWUF0sp98GyxIvLXYIWqSZ3nX_j_q4UN/pubhtml) publiée par l’[Alliance nationale des connaissances et langues autochtones (ANCLA)](https://nationalindigenousknowledgeandlanguagealliance.home.blog/) via Google Drive est un exemple de concrétisation de ces travaux  d’ouverture des données entrepris pour permettre une meilleure prise en  compte et représentation des Autochtones dans les bibliothèques, les  archives et les institutions liées à la mémoire. Des bénévoles des  treize provinces canadiennes ont travaillé, main dans la main, avec un  groupe de la FCAB, pour parvenir à la production de vedettes-matières.  Ce document évolutif, constamment mis à jour, apporte des informations  et des précisions sur des noms dont l’emploi est préconisé par les  communautés concernées elles-mêmes.

https://docs.google.com/spreadsheets/d/e/2PACX-1vSOKcm9HB-28iSqNN3sQd5hV7bMLMGpCeGL0dkQgyg2AiZAMWUF0sp98GyxIvLXYIWqSZ3nX_j_q4UN/pubhtml

---

background-image: url(imagesMSL/indigitization.png)

Indigitization. « Indigitization ». Consulté le 17 octobre 2023. https://www.indigitization.ca.

---

background-image: url(imagesMSL/sustainableNetwork.png)

« The Sustainable Heritage Network ». Consulté le 17 octobre 2023. https://sustainableheritagenetwork.org.

---

template: inverse

class: center middle

## Une exigence d’ouverture

???

Musées et thesaurisation

- Revendication citoyenne sur les communs
- Contexte plus général de l’Open data

Nouveaux enjeux pour les institutions patrimoniales et culturelles liés à l’ouverture des données et la diffusion des contenus.

Nouveaux régimes de circulations des artefacts culturels qui entraînent de nouvelles formes d’engagement avec ces contenus qui doivent désormais être intégrés aux politiques institutionnelles et leur écosystème.

Modification profonde des attitudes et des pratiques.

Lien avec la culture libre, nouvelles communautés.
Émergence d’une société civile et d’organisation qui réclament de plus en plus une participation active.

---

background-image: url(imagesMSL/licencesCC.jpg)

[http://framabook.org/optionlibre-dubonusagedeslicenceslibres/](http://framabook.org/optionlibre-dubonusagedeslicenceslibres/)

???
Dépôt volontaire

Nombreuses licences.
Comment choisir

Les licences Creative Commons constituent un ensemble de licences régissant les conditions de réutilisation et/ou de distribution d'œuvres (notamment d'œuvres multimédias diffusées sur Internet). Élaborées par l'organisation Creative Commons, elles ont été publiées le 16 décembre 2002.

[http://framabook.org/optionlibre-dubonusagedeslicenceslibres/](http://framabook.org/optionlibre-dubonusagedeslicenceslibres/)

ODBL
Open Knowledge Fundation

---

## La notion de GLAM

### .red[GLAM], acronyme de .red[G]alleries, .red[L]ibraries, .red[A]rchives et .red[M]useums.

???

**GLAM** est un acronyme anglais pour Galleries, Libraries, Archives and Museums (en français Galeries, Bibliothèques, Archives et Musées).

Plus généralement, il désigne des institutions publiques chargées de la collecte d'éléments du patrimoine culturel et historique. Le terme est apparu dans les années 2000.

Son émergence traduit notamment la prise de conscience par ces diverses institutions que leurs rôles et leur but convergeaient. Cette convergeance étant devenue de plus en plus visible à l’ère du numérique et de la publications des collections en ligne. Institutions fondées sur des modèles épistémologiques semblables, revenant à leur unité originelle (bibliothèque d’Alexandrie, musée, cabinet de curiosité). Des lieux qui préservent et rendent accessibles au public des artefacts historiques à valeur patrimoniale.

En décembre 2010, de premiers événements GLAM ont ainsi été programmés à Londres et Paris, et plus tard d'autres ont suivi dans le monde, dont en France.

1	http://uk.wikimedia.org/wiki/GLAM-WIKI
2	http://rencontres.wikimedia.fr/index.php?title=Accueil [archive]
3	À partir de 2013, ils sont relatés dans la revue Wiki Revue ; Wiki Revue janvier - mars 2013 (PDF, 12p)

cf. Deanna Marcum, Archives, Libraries, Museums:
Coming Back Together? Information & Culture: A Journal of History, Volume 49, Number 1, 2014 [https://muse.jhu.edu/journals/libraries\_and\_culture/v049/49.1.marcum.html](https://muse.jhu.edu/journals/libraries_and_culture/v049/49.1.marcum.html)

---

## La notion de « communs »

#### des bien partagés

#### un mode de gouvernance collectif

#### vs enclosure

Garrett Hardin, « La tragédie des communs »

Elinor Ostrom, « Gouvernance des biens communs »

???

Le **bien commun** est une notion théologique, philosophique et politique qui désigne l'idée d'un bien partagé par les membres d'une même communauté, au sens spirituel et moral du mot "bien" aussi bien qu'au sens matériel et pratique (les biens).

Ce concept semble intuitivement facilement compris, mais s'avère difficile à définir et parfois à traduire (ex l’anglais ne distingue pas facilement le "collectif" du "public", et le mot "commun" est très polysémique en français).

Au pluriel, les biens communs désignent des ressources matérielles ou non, qui sont ou devraient être partagées par tous (l'information, par exemple).

En droit

Le « bien commun » est plus ou moins explicitement pris en compte ou défendu par le droit coutumier et/ou certains dispositifs réglementaires classiques (souvent confondu avec l'intérêt public ou l'intérêt général, par opposition aux intérêts particuliers) et s'insère généralement dans un dispositif plus ouvert de négociation locale qui tend aussi depuis plusieurs décennies à devenir global et mondial

En 1968, le socio-biologiste **Garrett Hardin** postule qu'un accès libre au bien collectif conduit inévitablement à une **« tragédie des communs »**, sauf si (selon lui) un système en régule la consommation ou l'exploitation par un contrôle de la natalité et de la démographie, la nationalisation de ces biens ou leur privatisation.

Ce modèle, qui a conduit à la surexploitation de nombreuses ressources naturelles et à l'aggravation du dérèglement climatique et à une croissance des inégalités, sera ensuite dénoncé par l'économiste et politologue américaine **Elinor Ostrom** qui propose une théorie alternative à la fois au tout-marché et au tout-État, au profit de l'action collective et d'une gestion plus collaborative et négociée des biens communs et des biens publics (matériels ou immatériels). Elle inscrit ce courant dans une **« nouvelle économie institutionnelle »**30, notamment précisée en 1990 dans son livre **« Gouvernance des biens communs »**31.
Selon E. Ostrom, ce qui différencie le commun et le collectif et/ou public aurait son origine dans une décision et des choix de type politique et collectifs, quel que soit l’échelon considéré, du local au global.

[https://fr.wikipedia.org/wiki/Bien\_commun](https://fr.wikipedia.org/wiki/Bien_commun)

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

background-image: url(imagesMSL/openData.jpg)

[https://www.w3.org/DesignIssues/LinkedData.html](https://www.w3.org/DesignIssues/LinkedData.html)

???

Tim Berners-Lee
Date: 2006-07-27, last change: $Date: 2009/06/18 18:24:33 $
[https://www.w3.org/DesignIssues/LinkedData.html](https://www.w3.org/DesignIssues/LinkedData.html)

1	Use URIs as names for things
2	Use HTTP URIs so that people can look up those names.
3	When someone looks up a URI, provide useful information, using the standards (RDF*, SPARQL)
4	Include links to other URIs. so that they can discover more things.

## Open Data et Open government

Dans les années 50 aux États-Unis un jeune élu démocrate John E. Moss a commencé à militer en faveur de l’accès à l’information dans le contexte d’une amérique marquée par le maccarthysme. Nommé à la tête d’un nouveau sous-comité de l’information gouvernementale en 1955, il fut l’auteur d’un rapport sur l’accès à l’information gouvernementale. Sa proposition d’une loi le Freedom of Information Act fut adoptée sous l’administration Johnson en 1965 et votée en 1966. Cette loi servit de modèle à plusieurs législations similaires dans le monde (Suède 1970, France 1978, Pays-Bas 1980, Australie 1982, Canada 1983, Royaume-Uni 2000).

En décembre 2007, intervint une réunion à Sebastopol, une ville au Nord de San-Francisco, destinée à dégager la notion de données publiques ouvertes en vue de la faire adopter par les candidats à l’élection présidentielle américaine de 2008. Les participants à cette réunion étaient issus des mouvement du logiciel et de la culture libre qui se trouvaient au cœur de l’innovation depuis une quinzaine d’années (Fondation Apache, l’Encyclopédie collaborative Wikipedia, SourceForge, O’Reilly, etc.). Participèrent notamment à cette réunion des activistes comme le juriste Lawrence Lessig, l’éditeur Tim O’Reilly, ou encore le jeune activiste Aaron Swartz. Mais aussi des entrepreneurs qui utilisaient des données publiques pour fournir de nouveaux services numériques tels qu’Adrian Holovaty, fondateur du service d’informations localisées EveryBlock, ou le Britannique Tom Steinberg, initiateur du site FixMyStreet (Chignard 2013). 

Cette réunion permit de formaliser des principes encore utilisés aujourd’hui pour définir et d’évaluer ce qui constitue des données publiques ouvertes.

> Ces principes portent à la fois sur une idée fondamentale et sur des manières de faire. L’idée fondamentale, c’est qu’au même  titre que les idées scientifiques les données publiques sont un bien  commun. Les manières de faire portent principalement sur le partage et  l’utilisation de ce bien commun. (Chignard 2013)

Comme le relève Simon Chignard ces idées étaient directement inspirées des pratiques de la communauté du logiciel open source qui s’était organisée autour de trois notions : l’**ouverture, la participation et la collaboration**. Cette culture s’était développée dans le domaine du logiciel gratuit et libre où les programmeurs étaient invités à contribuer publiquement par l’intermédiaire de plateformes de partage de code informatique. Le partage des codes sources permettait de bénéficier du travail des autres en échange de droits concernant sa reproduction. Un dispositif fondé sur la transparence et la méritocratie qui garantissait l’amélioration du logiciel et la capitalisation sur les développements réalisés dans un travail de pair à pair fondé sur la compétence et la réputation. 

La participation de plusieurs personnalités du logiciel libre à cette réunion témoigne directement d’une sorte de filiation entre les principes du logiciel libre et ceux de l’open data. Pour Tim O’Reilly, il s’agissait en réalité d’appliquer aux affaires publiques les principes de l’open source et ses méthodes de travail. Les résultats de cette initiative dépassèrent les espérances puisque lorsque Barack Obama prit ses fonctions en 2008, il signa trois mémorandums dont deux concernaient le gouvernement ouvert (*open goverment*). Une politique qui se réclamait de la culture de l’*open source* et ses principes de transparence, de participation et de collaboration et qui reposait notamment sur le pilier de l’*open data*.

Qu’il s’agisse d’open source, d’open gouvernement ou d’open data, l’ouverture apparaît comme le vecteur commun de ces démarches. « Elle représente à la fois une philosophie d’action et une profession de foi, une pratique et un objectif. » (Chignard 2013)

En France, la donnée publique est aujourd’hui définie par la loi et concerne les acteurs publics ou privés qui interviennent dans le cadre de mission de services public. Les lois comme le *Freedom Information Act* aux États-Unis ou la loi CADA (Commission d’accès aux documents administratifs) de 1978 en France, associaient à ces données un droit d’accès et de réutilisation. L’approche de l’open data tente d’introduire un renversement de logique en proposant une publication par défaut des informations publiques, avant même que celles-ci soit réclamées par des tiers.

En 2009, Tim Berners-Lee fit de l’ouverture une injonction dans le cadre d’une conférence TED avec son « We want raw data, now ! » Une telle ouverture implique un changement culturel majeur parmi les acteurs, une sorte de lâcher prise qui ne va pas sans susciter de nombreuses craintes ou réticences qui expliquent la difficulté de la mise en place de ces politiques. Cette approche répond aux impératifs de transparence et d’*accountability* poussés par des préoccupations démocratiques ou une volonté de moderniser l’action publique. L’*open data* peut, en effet, être conçu comme une réponse à une époque de défiance de la part des citoyens vis-à-vis des institutions et de leurs représentants. Mais il s’inscrit également parfaitement dans une idéologie néo-libérale et néo-managériale qui revendique que les entreprises puissent tirer un bénéfice commercial de données publiques et une amélioration de la gouvernance des affaires publiques. Au point qu’un certain nombre de ses promoteurs comme Lawrence Lessig ou Beth Noveck ont depuis pris leur distance avec l’idée d’une transparence radicale.

Janvier 2010 data.gov.uk lancée comme plateforme d’open data au Royaume-Uni avec le support de Tim Berners Lee.

https://datacatalogs.org/

### Le Partenariat pour un gouvernement ouvert (PGO)

- « Open Government Declaration | Open Government Partnership ». 2011. Open Government Partnership. https://www.opengovpartnership.org/process/joining-ogp/open-government-declaration/.

Fondée en 2011 par huit gouvernements (Déclaration endossée par 75 organisation gouvernementales en 2011 (Afrique du Sud, Brésil,  États-Unis, Indonésie, Mexique, Norvège, Philippines et Royaume-Uni), le Partenariat pour un Gouvernement Ouvert (PGO) encourage les gouvernements à travailler en partenariat avec la  société civile et le secteur privé dans le but de créer et de mettre en  œuvre des politiques ouvertes ambitieuses. Depuis sa création en 2011, 76 pays ont adhéré au partenariat. Le Canada y joue un rôle de leadership clé et en a assumé la fonction de président principal en octobre 2018. [Les priorités sous son leadership sont notamment l’inclusion, la participation et l’incidence du Partenariat](https://ouvert.canada.ca/fr/contenu/le-role-du-canada-titre-de-copresident-2018-2019-du-partenariat-pour-un-gouvernement-ouvert).

@todo faire le parallèle avec la politique britannique et le recrutement de Tim Berners Lee

### Open data au Canada

Le gouvernement fédéral canadien s’est fortement engagé dans une politique de données ouvertes et de gouvernement ouvert. En 2016, le pays était classé deuxième pour la publication de données gouvernementales dans le baromètre de la fondation pour les données ouvertes du World wide web (https://opendatabarometer.org), devant la France et les États-Unis.

Dès 2010, le Canada établi une politique fondée sur les principes de Sebastopol. Placée sous la responsabilité du président du Secrétariat du Conseil du Trésor du Canada, un pilote de publication de données fut lancé en 2011 suivi d’un plan de trois ans destiné à augmenter le nombre de jeux de données publiés et améliorer l’implémentation technique de la plateforme. Une nouvelle version du portail de données fut ainsi publiée en juin 2013.

Le 9 octobre 2014, le gouvernement publia une Directive sur le gouvernement ouvert qui incluait une politique d’ouverture par défaut. Et le 6 novembre 2014, le gouvernement annonça un second plan d’action pour le gouvernement ouvert suivi d’un troisième plan d’action bisannuel publié le 15 juillet 2016. Le 12 mars 2018, le gouvernement publia une Charte des données ouvertes, et la même année son quatrième pan d’action.

- https://open.canada.ca

De nombreux plans provinciaux ont également été mis en place comme par exemple au Québec à partir de 2012, et en Colombie Britannique et au Saskatchewan dès 2011. Plusieurs villes comme ont également développé ce genre d’initiatives (Edmonton, Ottawa, Montreal, etc.). Soixante six municipalités disposaient d’un portail de données ouvertes au Canada en 2019.

- https://www.donneesquebec.ca
- https://open.canada.ca
- http://donnees.ville.montreal.qc.ca

France

- https://www.data.gouv.fr
- http://data.culture.fr/thesaurus/
- https://francearchives.fr
- https://opendata.paris.fr

https://www.data.gov

https://www.opendataimpactmap.org

http://opendatahandbook.org/

## L’Open Science

- Wilkinson, Mark D., Michel Dumontier, IJsbrand Jan Aalbersberg, Gabrielle Appleton, Myles Axton, Arie Baak, Niklas Blomberg, et al. 2016. « The FAIR Guiding Principles for Scientific Data Management and Stewardship ». *Scientific Data* 3 (mars) : 160018. https://doi.org/10.1038/sdata.2016.18.

---

background-image: url(imagesMSL/OpenGLAM-logo.png)

???

**GLAM** est un acronyme anglais pour Galleries, Libraries, Archives and Museums (en français Galeries, Bibliothèques, Archives et Musées).

Galleries, Libraries, Archives, Muséum. C’est à dire une part notable du secteur du patrimoine culturel. En quelques années, le terme est devenu une appellation parapluie pour les Organismes mémoriels. Son concept s‘est consolidé à travers des initiatives numériques comme Europeana, le portail européen des bibliothèques, musées et archives européennes, la Digital Public Library of America, une initiative équivalente de l’Université Harvard, et les GLAM-Wiki qui coopèrent avec les institutions culturelles à travers le monde pour partager des ressources sur Wikipédia.

**GLAM** est un acronyme anglais pour Galleries, Libraries, Archives and Museums (en français Galeries, Bibliothèques, Archives et Musées).

Plus généralement, il désigne des institutions publiques chargées de la collecte d'éléments du patrimoine culturel et historique. Le terme est apparu dans les années 2000.

Son émergence traduit notamment la prise de conscience par ces diverses institutions que leurs rôles et leur but convergeaient. Cette convergeance étant devenue de plus en plus visible à l’ère du numérique et de la publications des collections en ligne. Institutions fondées sur des modèles épistémologiques semblables, revenant à leur unité originelle (bibliothèque d’Alexandrie, musée, cabinet de curiosité). Des lieux qui préservent et rendent accessibles au public des artefacts historiques à valeur patrimoniale.

En décembre 2010, de premiers événements GLAM ont ainsi été programmés à Londres et Paris, et plus tard d'autres ont suivi dans le monde, dont en France.

1   http://uk.wikimedia.org/wiki/GLAM-WIKI
2   http://rencontres.wikimedia.fr/index.php?title=Accueil [archive]
3   À partir de 2013, ils sont relatés dans la revue *Wiki Revue* ; Wiki Revue janvier - mars 2013 (PDF, 12p)

cf. Deanna Marcum (2014). « Archives, Libraries, Museums: Coming Back Together? » *Information & Culture: A Journal of History*, Volume 49, Number 1. <https://muse.jhu.edu/journals/libraries_and_culture/v049/49.1.marcum.html>

### OpenGLAM

OpenGLAM, mouvement international pour faire de l’ouverture le standard pour le secteur des GLAM. Culture du partage et culture internet.

Cf. OKF

> “Galleries,  libraries,  archives  and museums  have  an  important  role in  supporting  the  advance  of  hu-manity’s  knowledge.  They  are  the custodians of our cultural heritage and in their collections they hold the record  of  humankind.  The  internet aªords  cultural  heritage  institu-tions a radical new opportunity to engage global audiences and make their collections more discoverable and connected than ever, allowing users  not  only  to  enjoy  the  riches of the world’s  memory  institutions, but  also  to  contribute, participate and  share.”  http://openglam.org/ principles/

- attitude ouverte et accueillante à l’égard du public et de ses contributions
- ouverture des contenus (open access), images et données

Historienne de l’art, explique efforts pour transformer les musées pour renforcer position de l’histoire de l’art. La question de l'accès et de sa démocratisation.

Lawrence Lessig, Clay Shirky, Chris Anderson, Tim O’Reilly, Don Tapscott, and Anthony Williams - some of the most well-established thinkers within Internet culture and economics. Don Tapscott, Anthony D Williams, et la notion de Wikinomics

---

background-image: url(imagesMSL/communia.png)

???

background-image: url(imagesMSL/okf.png)

[The Open Knowledge Foundation](http://www.okfn.org/ "The Open Knowledge Foundation")

L’**Open Knowlegde Foundation** est une association à but non lucratif de droit britannique qui promeut la culture libre et en particulier les contenus libre et l’open data (les données ouvertes).
Elle a été créée le 24 mai 2004 à Cambridge au Royaume-Uni.

Elle a notamment publié une définition des savoirs libres (sur le modèle des définitions GNU) _Open definition_.

Elle est à l’origine de divers projets tels

- [CKAN](https://fr.wikipedia.org/wiki/CKAN) un logiciel permettant la publication de données ouvertes utilisé par de nombreux organismes
- _Where does my money go_ un projet de suivi des dépenses publiques.
- Open Database Licence (ODbL)
- Public Domain Review
- School of Data

La fondation milite pour la culture libre, offre du conseil dans le choix des licences et publie donc divers outils techniques.

L’association compte aujourd’hui plus de 24 chapitres et groupes régionaux à travers le monde.

Public Domain Review

background-image: url(imagesMSL/savoirscom1.jpg)

[http://www.savoirscom1.info](http://www.savoirscom1.info)
Bien Com1 militantismes

Création septembre 2012

SavoirsCom1 est un collectif engagé pour le développement de politiques et d’initiatives liées aux communs de la connaissance. Nous agissons selon notre Manifeste. Nous sommes un collectif indépendant orienté vers l’action et organisé de manière horizontale.

---

background-image: url(imagesMSL/sharing.jpg)

???

## Sharing is Caring

Rêve des Lumières et formidable opportunité d’un monde connecté.

Passage du partage de fichier au monde de la culture. Que se passe-t-il quand partage.

Anthologie issue des séminaires de 2011 et 2012. Publiée sous Licence CC BY 4.0

Galeries nationales du Danemark, principal musée d’art du pays.

**We must think like users to incorporate not just the technologies themselves**

> Technology should not govern the museums’ work. But in order to learn and understand how we can use new technologies and benefit from the opportunities they open up to us we must ex -plore and incorporate not just the technologies themselves, but also the changes in behaviour and expectations they prompt in users. We must think like users.

---

background-image: url(imagesMSL/displayAtYourOwnRisk.png)

.footnote[https://displayatyourownrisk.org/]

???

*Display At Your Own Risk* (DAYOR) is a research-led  exhibition experiment featuring digital surrogates of public domain  works of art produced by cultural heritage institutions of international repute. The project includes a Gallery Exhibition as well as an open  source version of that exhibition intended for public use.

**Gallery Exhibition**

The exhibition [opened](http://displayatyourownrisk.org/opening/) at The Lighthouse in Glasgow on 8 June 2016 for one night only. The  works featured in the exhibition were curated from the online  collections of internationally renowned cultural institutions. The [digital surrogate](http://displayatyourownrisk.org/digital-surrogates/) made available on the institution’s website was printed to the original dimensions of the underlying object. As most institutions claim  copyright over the photographs they take of works in their collection,  the institutions themselves were credited as the author and/or copyright owner of these digital surrogates where appropriate. Information about  how the institution licenses the use of these surrogates – including  information about pricing where relevant – was also included within the  exhibition.

The exhibition is guided by a number of concerns. By printing the  digital surrogate to the work’s original dimensions, it invites  reflection on the nature and quality of the reproductions that  institutions make available online in place of the material object  within their care. It considers the meaning of concepts such as access,  transparency and user engagement in an age where digital collections are becoming increasingly relevant. And it explores tensions inherent in  the ownership and use of cultural heritage, as well as the validity of  the authorial claims that institutions assert over these digital  surrogates – surrogates that are often viewed as new and independent  assets.

---

background-image: url(imagesMSL/nefertiti.png)

.footnote[Jan Nikolai Nelles, Nora Al-Badri. The Other Nefertiti. 2015. http://nefertitihack.alloversky.com/]

---

## La notion de « Fair use » ou de « Fair dealing »

#### « Fair dealing » et droit canadien

#### Canada : « utilisation équitable » art.29 et suiv. L.R. 1985, ch. C-42

???

Droit d’auteur et restrictions aux utilisations légitimes

émergence de la notion de « fair use » ou d’usage loyal, raisonnable ou acceptable.

Il s’agit d’un ensemble de règles de droit, d'origine législative et jurisprudentielle, qui apportent des limitations et des exceptions aux droits exclusifs de l'auteur sur son œuvre (droit d'auteur). Il essaie de prendre en compte à la fois les intérêts des bénéficiaires des droits d'auteur et l'intérêt public, pour la distribution de travaux créatifs, en autorisant certains usages qui seraient, autrement, considérés comme illégaux.

- Quelques pays ont calqué leur loi sur le fair use américain ;
- La plupart des pays de common law ont une doctrine similaire, le fair dealing, qui se traduit par utilisation équitable.
- Au Canada : utilisation équitable art.29 et suiv. loi sur le droit d’auteur (L.R. 1985, ch. C-42) ;

Il s'agit fondamentalement de l'intention et de la motivation de l'usage ;

Critère de quantité et d’importance

Effet sur la valeur de l’œuvre

### exemple de Google

La Guilde des auteurs a engagé il y a huit ans contre Google un procès portant sur le programme de numérisation de livres dans les bibliothèques publiques américaines.

Selon la décision rendue par le juge Denny Chin le 14 novembre 2013, la base de données numérisées ainsi constituée respecte le fair use et permet aux « lecteurs, aux universitaires, aux chercheurs et à tout un chacun de découvrir des livres. Google Livres est devenu un outil important pour les bibliothèques8. » Selon le juge, le détournement des ventes qui serait facilité par Google n'est pas attesté : « Google Books fournit aux ouvrages un moyen d'être remarqués, autant que leur présentation en magasin8. »

Le président de la Guilde, Paul Aiken, a fait part de son désaccord avec cette décision « déclarant que cette mise en cause fondamentale du droit de copyright méritait l'examen d'une juridiction supérieure8. »

---

background-image: url(imagesMSL/wallace2019.png)

.footnote[Pavis, Mathilde, et Andrea Wallace. 2019. « Réponse au Rapport Sarr-Savoy : Déclaration sur la numérisation, les droits de propriété intellectuelle et le libre accès du patrimoine culturel africain et des archives connexes ». *JIPITEC* 10 (2). https://www.jipitec.eu/issues/jipitec-10-2-2019/4911.]

---

## Les principes de PCAP® des Premières Nations

https://fnigc.ca/fr/les-principes-de-pcap-des-premieres-nations/

> Les principes de PCAP® des Premières Nations déterminent comment les  données et les informations des Premières Nations seront collectées,  protégées, utilisées ou partagées. Ces principes, dont le sigle signifie la **propriété**, le **contrôle**, l’**accès** et la **possession**, sont un outil  visant à soutenir une gouvernance solide de l’information sur la voie de la souveraineté des Premières Nations en matière de données. Compte  tenu de la diversité au sein des nations et entre elles, les principes  seront exprimés et affirmés conformément à la vision du monde, aux  connaissances traditionnelles et aux protocoles respectifs des nations.

???

### OCAP

Brown, Deidre, et George Nicholas. « Protecting Indigenous Cultural Property in the Age of Digital Democracy: Institutional and Communal Responses to Canadian First Nations and Māori Heritage Concerns ». *Journal of Material Culture* 17, no 3 (1 septembre 2012): 307‑24. doi:[10.1177/1359183512454065](https://doi.org/10.1177/1359183512454065).

Question de l’ouverture et point de vue autochtone. Ne pas nuiore aux perspectives autochtones, valeurs et identité lorsque culture numérisée.

Graber and Burri-Nenova 2008, Dyson et al. 2007

Pas de différence entre propriété culturelle et propriété intellectuelle. Pas de séparations apsects tangibles ou intangibles.

/+ Conscience que nombreux aspects de leur patrimoine appropriés ou commodifiés.

> Few legal options are available, furthermore, to protect indigenous  cultural heritage. In Western law, protection of intellectual property  is based on property values and ‘rights’, and is concerned largely with  ‘things’; ownership is vested in individuals; and infringement results  in economic loss. Protection is through copyrights, patents and  trademarks, which have very specific applications. ‘Indigenous  intellectual property’, however, is situated in customary law and  culture, and based on social relations and responsibilities.

---

background-image: url(imagesMSL/care.png)

## CARE

.footnote[Global Indigenous Data Alliance. « CARE Principles of Indigenous Data Governance ». Consulté le 30 mai 2021. https://www.gida-global.org/care.]

---

background-image: url(imagesMSL/traditionalKnowledgeLabels.png)

.footnote[Traditional Knowledge (TK) Labels, https://localcontexts.org/tk-labels/]

???

> Les étiquettes de savoir traditionnel  (ST) sont des outils permettant aux communautés autochtones de lier  leurs protocoles internes d’accès et d’utilisation à tout patrimoine  culturel documenté qui circule sur une plateforme numérique extérieure  aux communautés. Les étiquettes ST favorisent l’adoption d’une stratégie pédagogique et informative envers les utilisateurs non membres des  communautés d’origine de ce patrimoine culturel. Elles permettent à ces  utilisateurs de mieux comprendre l’importance et la portée de ce  patrimoine culturel qui demeure signifiant pour les communautés  d’origine. L’étiquetage ST a été conçu pour identifier tout matériel  soumis à des restrictions spécifiques à une communauté et pour en  expliciter l’accès et l’utilisation. Ces restrictions s’appliquent plus  particulièrement au matériel de nature sacrée ou cérémoniale, au  matériel comportant des restrictions de nature genrée, à l’utilisation  saisonnière ou au matériel conçu spécifiquement à des fins de  sensibilisation. Les étiquettes ST peuvent également servir à ajouter de l’information « manquante », telle que le nom de la communauté qui est  le créateur ou le gardien culturel du matériel ainsi que la façon de  communiquer avec la famille, le clan ou la communauté concernée afin  d’obtenir les permissions appropriées.

---

template: inverse

class: center middle

# Bibliographie

---

# Bibliographie

- ICOM. Code de déontologie de l’ICOM pour les Musées. 2017. ISBN 978-92-9012-421-4 http://icom.museum/fileadmin/user_upload/pdf/Codes/ICOM-code-Fr-web.pdf
- Sanderhoff, Merete, and Michael Peter Edson, eds. *Sharing Is Caring: Openness and Sharing in the Cultural Heritage Sector ; [an Anthology]*. Copenhagen: Statens Museum for Kunst, 2014. http://www.smk.dk/en/about-smk/smks-publications/sharing-is-caring/
- Dubuc É et Turgeon L. 2004, Musées et Premières Nations, Anthropologie et sociétés, vol. 28, n° 2.
- Halpin, M. et Ames M. (1999). Musées et Premières Nations au Canada. Revue ethnologique française, T. 29, n° 3, p. 431-436.
- Moses, J. (1997). «Museum and Native Peoples Issues. An Ethical and Theoretical background for the care of Native North American Cultural Materials », ICOM. Ethnographie Conservation Newsletter, n° 16.
- Jamin, J. (1998). « Faut-il brûler les musées d'ethnographie ? », Gradhiva, n° 24, p. 65-69.

???

@todo Ajouter

Stacy Allison-Cassin, York University bibliothécaire LOD. A travaillé sur LCSH sujets indigènes, décolonisation des bibliothèques.

https://sacassin.blog.yorku.ca

https://nationalindigenousknowledgeandlanguagealliance.home.blog/2019/06/21/first-nations-metis-and-inuit-indigenous-ontologies-fnmiio/

https://nationalindigenousknowledgeandlanguagealliance.home.blog

Articles

## Douglas

Objets volés et importance des bases de données.

> We argue that high-quality digital representations of artworks must support the functionality of databases and reach a broad audience if cultural heritage is to be served.

développement multimedia

> This originated with the idea of convergence, a model that would challenge museums to reframe the role of the public in relation to larger policy goals as well as invite them to redefine virtual museum visitors as “members of the knowledge economy”.16

Google, qualité des images

Domaine public

Base de données des objets volés

Voici des liens vers les travaux de Hannah Turner, chercheuse sur les questions de décolonisation des bases de données : https://www.sfu.ca/ipinch/about/ipinch-people/associates/hannah-turner/http://www.tandfonline.com/doi/pdf/10.1080/01639374.2015.1010112?needAccess=true

http://onlinelibrary.wiley.com/doi/10.1111/muan.12118/full

http://onlinelibrary.wiley.com/doi/10.1111/muan.12122/full

Et le Bard Graduate Center :

https://www.bgc.bard.edu/ vidéos en ligne : https://www.youtube.com/user/bardgradcenter/videos les sujets sont très variés.



### Vermeylen, Saskia, et Jeremy Pilcher. « Let the Objects Speak: Online Museums and Indigenous Cultural Heritage ». *International Journal of Intangible Heritage* 4 (2009).

Dès les années 60 et le mouvement des droits civils, se fait jour aux US une critique des biais du musée. Depuis les années 70, toute une littérature pointe le rôle social que doivent remplir le musée. Cf. nouvelle définition.

Pearce 1994, Jones, 1993, Barringer & Flynn 1998, Simpson 2001, Stanley 2007.

Respect des droits autochtones Kelly et Gordon 2002 . Butts 2002

Nouvelle muséologie de Peter Vergo 1997. appelant transformation du musée d’un site d’adoration à un site qui s’engage dans des discours multiples.

Concept de musée indigène (Stanley 2007)

Exposition The Spirit Sings : artistic Tradition of Canada’s First Peoples (Gibbons 1997). Pas de curator autochtone parmi les 6. Débat. 1992 Turning the Page.

Dans les musées australiens, Rencontre du Crocodile Hole à Kimberley, où débat ainés sur pratiques culturelles, tournant. *Report of the State Task Force for Museums Policy* 1992 et développement de documents de politique *Previous Possessions, New Obligations : Policies for Museums in Australia and Aboriginal and Torres Strait Islander People* en 1993 (Galla 1994, 2008)

National Museum of The American Indian à Washington (Shelton 2006) importance du culturel sur la préservation.

Rappatriation, mais aussi besoin de facilitation agency et dialogue. Vie des communautés souvent « reduced to an abstract set of largely arbitrary material items displayed without much sense of mening. » (Stanley 2007)

Cultures mortes.

Question des objets, et de la manière dont incorporent des valeurs culturelles.

Utilisation de la plateforme du web comme possibilité de dialogue. Cf. Convention sur le patrimoine immatériel

### Frank, Paul. « CaMMS Subject Analysis Committee ». LC Policy, Training, and Cooperative Programs Division, 2022. https://connect.ala.org/core/discussion/sac-2022-annual-meeting-lc-ptcp-report.

Report from the Library of Congress Liaison submitted by Pual Franck

LCSH

tribal groupings headings

septembre Slaves to Enslaved persons

Conservation d’une note historique

### UN Declaration on the Rights of Indigenous Peoples, 2007

Reconnaissance de la voix des premiers concernés par l’ICOM

### Indigitization. « Indigitization ». Consulté le 17 octobre 2023. https://www.indigitization.ca/.

> Indigitization is a collaborative initiative between BC Indigenous groups and academic partners from the University of British Columbia and the University of Northern British Columbia to facilitate capacity building in Indigenous information management.

https://www.indigitization.ca/toolkit/managing-digital-information/#metadata

« Section H: Metadata and Description ». Indigitization Toolkit. Indigitization, 2020. https://library-indigitization-2020.sites.olt.ubc.ca/files/2020/06/H-2018.pdf.

H3: FIRST NATIONS CONTROLLED VOCABULARY BC First Nations Subject Headings, 2009 ( Xwi7xwa Library, First Nations House of Learning) URL: http://xwi7xwa.library.ubc.ca/files/2011/09/bcfn.pdf Last access: January 12, 2018. 

A working document from the Xwi7xwa Library, University of British Columbia that combines Xwi7xwa, Library of Congress, and other subject headings. 

Ngā Ūpoko Tukutuku | Maori Subject Headings, 2017 (LIANZA, Te Rōpū Whakahau, and the National Library of New Zealand) URL: http://natlib.govt.nz/nga-upoko-tukutuku Last access: January 12, 2018. 

Ngā Ūpoko Tukutuku has been developed as part of the Māori Subject Headings Project jointly sponsored by LIANZA, Te Rōpū Whakahau and the National Library of New Zealand. The list of over 1,000 headings and their associated references is appropriate for use at a public library level. As more terms are developed they will be added to the list. 

Pathways: AIATIS Thesauri, 2010 (Australian Institute of Aboriginal and Torres Strait Islander Studies) URL: http://www1.aiatsis.gov.au/thesaurus/ Last access: January 12, 2018. 

Pathways contains headings for place names, language groups and people, and subjects relating to Australian Aboriginal and Torres Strait Islander studies. These headings are used to describe all items held in the AIATSIS Catalog. 

Words First: An Evolving Terminology Relating to Aboriginal Peoples in Canada, 2002 (Indian and Northern Affairs Canada) URL: http://publications.gc.ca/site/eng/264091/publication.html Last access: January 12, 2018

The purpose of Words First: An Evolving Terminology Relating to Aboriginal Peoples in Canada is to provide writers with background information and guidance on appropriate word usage and style issues.

### Vérité et réconciliation

### Nouvelle politique AAM

### Bénin

### OCAP

Brown, Deidre, et George Nicholas. « Protecting Indigenous Cultural Property in the Age of Digital Democracy: Institutional and Communal Responses to Canadian First Nations and Māori Heritage Concerns ». *Journal of Material Culture* 17, no 3 (1 septembre 2012): 307‑24. doi:[10.1177/1359183512454065](https://doi.org/10.1177/1359183512454065).

Question de l’ouverture et point de vue autochtone. Ne pas nuiore aux perspectives autochtones, valeurs et identité lorsque culture numérisée.

Graber and Burri-Nenova 2008, Dyson et al. 2007

Pas de différence entre propriété culturelle et propriété intellectuelle. Pas de séparations apsects tangibles ou intangibles.

/+ Conscience que nombreux aspects de leur patrimoine appropriés ou commodifiés.

> Few legal options are available, furthermore, to protect indigenous  cultural heritage. In Western law, protection of intellectual property  is based on property values and ‘rights’, and is concerned largely with  ‘things’; ownership is vested in individuals; and infringement results  in economic loss. Protection is through copyrights, patents and  trademarks, which have very specific applications. ‘Indigenous  intellectual property’, however, is situated in customary law and  culture, and based on social relations and responsibilities.

Reciprocal Research Network (RRN) is an innovative partnership between the Musqueam Indian Band, the Sto:lo Nation and Sto:lo Tribal Council, the U’mista Cultural Society, and the University of British Columbia’s Museum of Anthropology, which was developed ‘to facilitate reciprocal and collaborative research’.5

Dyson L, Henriks M and Grant S (2007) Information Technologies and Indigenous Peoples. Hershey, PA: Information Science Publishing.

Gillespie T (2007) Wired Shut: Copyright and the Shape of Digital Culture. Cambridge, MA: MIT Press. Graber C and Burri-Nenova M (eds) (2008) Intellectual Property and Traditional Cultural Expressions in a Digital Environment. Cheltenham: Edward Elgar.

Johnson V (1996) Copyrites: Aboriginal Art in the Age of Reproductive Technologies. (touring exhibition catalogue). Sydney: National Indigenous Arts Advocacy Association and Macquarie University.
