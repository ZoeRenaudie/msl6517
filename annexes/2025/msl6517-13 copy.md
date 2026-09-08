title: MSL6517-10
description: emchateau UdeM
theme: presentation/theme/remark-dark-em.css
name: inverse
layout: true
class: inverse

---

name: index

class: center middle




---

wikidata
titre, description, étiquettes multilingues. Exercice : créer un item pour une œuvre contemporaine ou exposition.
Ajouter des propriétés : date de naissance, nationalité, créateur, lieu d’exposition. Ajouter plusieurs valeurs si nécessaire. Liens et relations	Ajouter relations : lien œuvre → artiste, exposition → lieu, exposition → œuvre. Montrer comment les QID permettent de relier les items.

Questions et bonnes pratiques	
Vérifier doublons, 
importance des sources, 
introduction à SPARQL pour interroger Wikidata. 

Conseils pour documentation patrimoniale.

Mysql
### Pré-requis (en ligne)

* **DB Fiddle (MySQL 8.x)**
  [https://dbfiddle.uk/g2u6-4AX](https://dbfiddle.uk/g2u6-4AX)

  * Colonne de gauche : **Schema SQL**
  * Colonne de droite : **Query SQL**

Dans dbfiddle :

* tout le schéma (CREATE TABLE, INSERT, VIEW) va **dans Schema SQL**
* les SELECT vont **dans Query SQL**


---

# Pérennisation de l’information numérique

### MSL6517 – automne 2023 | Emmanuel Château

.footnote[<https://studium.umontreal.ca/course/view.php?id=254809>]

---

layout: false

### Digital Heritage

- UNESCO (2003). « Charte sur la conservation du patrimoine numérique », *Organisation des Nations Unies pour l’éducation, la science et la culture*. <http://portal.unesco.org/fr/ev.php-URL_ID=17721&URL_DO=DO_TOPIC&URL_SECTION=201.html>
- UNESCO (2003). *Directives pour la sauvegarde du patrimoine numérique*. Paris : Organisation des Nations Unies pour l’éducation, la science et la culture, 198 p. <http://unesdoc.unesco.org/images/0013/001300/130071f.pdf>
- UNESCO (2012). *Déclaration de Vancouver*. Vancouver : Organisation des Nations Unies pour l’éducation, la science et la culture et University of British-Columbia, 5 p. <http://www.unesco.org/new/fileadmin/MULTIMEDIA/HQ/CI/CI/pdf/mow/unesco_ubc_vancouver_declaration_fr.pdf>
- UNESCO (2016). « Concept de patrimoine numérique », *Organisation des Nations Unies pour l’éducation, la science et la culture*. <http://www.unesco.org/new/fr/communication-and-information/access-to-knowledge/preservation-of-documentary-heritage/digital-heritage/concept-of-digital-heritage>
- UNESCO (2016). « Concept de préservation numérique », *Organisation des Nations Unies pour l’éducation, la science et la culture*. <http://www.unesco.org/new/fr/communication-and-information/access-to-knowledge/preservation-of-documentary-heritage/digital-heritage/concept-of-digital-preservation>
- UNESCO (2016). « Patrimoine numérique », *idem*. <http://www.unesco.org/new/fr/communication-and-information/access-to-knowledge/preservation-of-documentary-heritage/digital-heritage>

???

Face à l’accroissement des ressources numérisées par le monde muséal, la question de la conservation de ces ressources a rapidement émergée comme une question cruciale à raison des investissements réalisés par les institution pour la numérisation de leur patrimoine.

Notion de Digital Heritage

- En 2003, l’UNESCO a élaboré une Charte sur la conservation du patrimoine numérique

- Cette prise de conscience est réitérée avec la publication de la déclaration de Vancouver en 2012 qui fit suite à la conférence internationale La mémoire du monde à l’ère numérique : numérisation et conservation

  Les principes directeurs de cette charte, visent «  l’adaptation et […] l’élargissement des mesures existantes en ce domaine » (UNESCO, 2016 c) et suggèrent une vision de la préservation numérique qui ne se limite plus à une simple suite de procédures et de solutions technologiques, mais qui introduit une responsabilité sociétale.

> Le patrimoine numérique est constitué de matériaux fondés sur l’informatique, d’une
> valeur durable, qu’il est nécessaire de conserver pour les générations futures.
> Il émane de communautés, de régions, d’industries et de secteurs différents.
> Tous les matériaux numériques ne sont pas de valeur durable, mais ceux qui le
> sont exigent des méthodes actives de préservation si l’on veut que la continuité
> du patrimoine numérique soit assurée. 
>
> Unesco 2016

Appelle donc une action de préservation active.

Notion de digital stewardship (Brian Lavoie et Lorcan Dempsey 2004). Approche systémique de la conservation.

- Digital Preservation for Libraries, Archives, & Museums (Corrado et Moulaison, 2017) 
- À la fine pointe du monde numérique : possibilités pour les institutions de la mémoire collective au Canada (CAC, 2015)

La préservation numérique peut être comprise comme un ensemble d’activités, de procédés et de politiques qui visent à assurer l’authenticité et l’accessibilité perpétuelle aux ressources numériques (UNESCO, 2016 b ; Library of Congress, n.d ; Digital Preservation Coalition, 2015).

> Digital Asset Management (DAM) is a collective term applied to the process
> of storing, cataloguing, searching and delivering computer files (or digital
> assets). […] Digital Asset Management (DAM) systems centralise assets and establish a systematic approach to ingesting assets so they can be located more easily and used appropriately. (Digital Asset Management News, 2016) 

Bruno Bachimont, et archivage numérique. Problème principal que les données sont codées. Aussi la question de la pérennisation de l’information numérique est-elle directement liée à la question des métadonnées.

---

## La distinction .red[numérique] vs .red[analogique]

???

Afin de proposer une définition plus spécifiquement technique du numérique, il convient pour commencer, d’aborder une distinction fondamentale qui est sous-jacente à la technologie numérique et qui justifie souvent la réunion d’un ensemble de technologies et de médias variés sous le concept de « numérique ». **Il s’agit de la distinction entre le numérique et l’analogique.**

Que signifie pour vous cette distinction ?

--

count: false

### Analogique

Qui représente, traite ou transmet des données sous la forme de variations d’intensités continues.

### Numérique (digital)

Qualifie les systèmes ou dispositifs n’employant que des valeurs discrètes traitées sous la forme de signaux binaires.

[Pour aller plus loin](http://www.parcoursnumeriques-pum.ca/pour-une-definition-du-numerique)

???

Une distinction fondamentale est sous-jacente à cette définition des nouveaux médias qui est aussi celle qui justifie la réunion d’un certain nombre de médias sous le concept de « numérique ». **Il s’agit de la distinction entre le numérique et l’analogique.**

L’analogique et le numérique désignent **deux procédés pour transporter et stocker des données** (de type audio , photo , vidéo…). L’analogique est né avec le début de l’électricité tandis que le numérique est apparu plus récemment à l’ère de l’informatique.

## Analogique

Analogique vient du grec _αναλογος_ (analogos), proportionnel.

Analogique se dit d’**une réalité qui se représente sous la forme d’un *continuum***. Par conséquent, un média analogique est un système qui représente, traite ou transmet des données sous la forme de variations d’intensités continues.

Analogue fait ici référence à des processus où un ensemble de propriétés physiques qui peuvent être stockées sous une autre forme physique, dite analogue.

On qualifie donc d’analogique **un système qui restitue une information en fonction de la variation d’une grandeur physique** (d’où le terme analogique, l’information évoluant de façon similaire à la source). Par exemple, les appareils photo dits argentiques, et qui utilisent une pellicule, capturent des images par un système analogique. En effet, la lumière qui pénètre à travers la chambre « impressionne » les substances chimiques sensibles à la lumière placées à la surface de la pellicule.

En fonction de son intensité selon les zones de l’image, le signal lumineux se trouve en quelque sorte enregistré, ou transformé en une oxydation des sels d’argent qui produit un analogue pictural de l’image.

## Numérique (ou digital)

Par opposition à l’analogique, **le numérique ou le digital, désigne un système ou un dispositif qui n’emploie que des valeurs discrètes habituellement traitées sous la forme signaux binaires**.

Le terme numérique vient du terme latin _numerus_ (« nombre », « multitude ») et signifie « représentation par nombres ». En mathématiques, on oppose ainsi le calcul numérique (l’arithmétique) au calcul littéral (par lettres, ou algèbre).

Le terme anglais « digital » vient du latin _digitus_ qui signifie « doigt » ; en anglais « digit » désigne un chiffre (0 à 9). Les autres langues romanes gardent le terme « digital », cf. italien, espagnol.

À la différence du français, le terme anglais est spécifique au traitement informatique et ne présente pas l’ambiguïté du français.

L’usage de « digital » en français est possible comme synonyme de « numérique ».

## Pour aller plus loin : 

http://www.parcoursnumeriques-pum.ca/pour-une-definition-du-numerique

---

background-image: url(imagesMSL/analogiqueVsNumerique.jpg)

## Phénomènes continus, Phénomènes discret

???

Une valeur discrète est une variable qui ne peut prendre des valeurs que dans un ensemble d’éléments définis à l’avance, tandis qu’une variable dite continue prendra ses valeurs dans un intervalle.

Les phénomènes qui nous entourent sont quasiment tous continus, c’est-à-dire que lorsque ces phénomènes sont quantifiables, ils passent d’une valeur à une autre sans discontinuité. 

Ce trait de la réalité physique a des conséquences pour la reproduction ou l’enregistrement des phénomènes.

Lorsque l’on veut reproduire un phénomène original, par exemple en l’enregistrant de la manière la plus efficace possible, **on parle d’enregistrement analogique si le support peut prendre des valeurs continues car ces valeurs seront analogues à celles du phénomène original**.

ex : la bande magnétique, le disque vinyle sont des supports analogiques

En revanche, le signal peut parfois prendre seulement des valeurs bien définies, en nombre limité, on parle alors de signal numérique.

La représentation d’un signal analogique se présente donc sous la forme d’une courbe, tandis qu’un signal numérique pourra être visualisé sous la forme d’un histogramme.

Dans une reproduction analogique, entre chaque point de cette courbe, il existe des points à l’infini – comme dans le cas d’une ligne droite continue : la courbe est donc « dense », dans le sens mathématique du mot, c’est-à-dire qu’elle ne comporte aucun saut.

Tandis que dans une représentation niveau, il y a un saut entre des valeurs séparées.

Vous pouvez immédiatement comprendre qu’un signal numérique est de ce fait beaucoup plus facile à reproduire qu’un signal analogique. On dit qu’elle est « sans perte ».

En même temps perte de qualité liée à la conversion numérique car elle implique une sorte de discrétisation, qui conduit à résoudre le signal en un ensemble de valeurs pré-définies à l’avance.

---

## Numérisation

La **numérisation** est une opération qui consiste à transformer quelque chose en données numériques.

- Passage de données **continues** du monde réel à un ensemble de valeurs **discrètes**.
- La transformation d’un signal **analogique** en signal **numérique** est appelée numérisation. 

**La numérisation implique deux activités : l’échantillonnage (en anglais *sampling*) et la quantification.**

- L’.red[échantillonnage] consiste à prélever périodiquement des échantillons d’un signal analogique. 

- La .red[quantification] consiste à affecter une valeur numérique à chaque échantillon prélevé.

  Cette quantification est une opération de discrétisation : on fait correspondre à un ensemble de valeurs continues des valeurs choisies dans un ensemble de valeurs fermé.

???

La **numérisation** est une opération qui consiste à transformer quelque chose en données numériques. Il peut s’agir de :

- la description d’un document physique par un fichier numérique ;
- la conversion d’un signal électrique analogique en un flux numérique ;
- l’entreprise de conversion des fonds documentaires datant des époques technologique précédentes.

La transformation d’un signal analogique en signal numérique est appelée numérisation. Lorsque l’on numérise des contenus, on passe de données continues du monde réel à un ensemble de valeurs discrètes.

**La numérisation implique deux activités : l'échantillonnage (en anglais sampling) et la quantification.**

- L’échantillonnage consiste à prélever périodiquement des échantillons d’un signal analogique. 
- La quantification consiste à affecter une valeur numérique à chaque échantillon prélevé.

Cette quantification est une opération de discrétisation : on fait correspondre à un ensemble de valeurs continues des valeurs choisies dans un ensemble de valeurs fermé.

idée de crible

La qualité du signal numérique dépendra de deux facteurs :

- la fréquence ou finesse de l’échantillonnage (appelé taux d’échantillonnage) : plus celle-ci est importante (c’est-à-dire que les échantillons sont relevés à de petits intervalles de temps) plus le signal numérique sera fidèle à l’original ;
- le nombre de bits sur lequel on code les valeurs (appelé résolution) : il s’agit en fait du nombre de valeurs différentes qu’un échantillon peut prendre. Plus celui-ci est grand, meilleure est la qualité.

Ainsi, grâce à la numérisation on peut garantir la qualité d’un signal, ou bien la réduire volontairement pour :

- diminuer le coût de stockage
- diminuer le coût de la numérisation
- diminuer les temps de traitement
- tenir compte du nombre de valeurs nécessaires selon l’application
- tenir compte des limitations matérielles

---

## Représentation numérique

### Une suite organisée d’unités binaires

- Les ordinateurs manipulent uniquement des données de type numérique (en l’occurence sous forme binaire)

- un `bit` peut avoir la valeur `1` ou `0` (*binary digit*)

- avec `2 bits` on peut avoir quatre états différents (`2 x 2`) : `00`, `01`, `11`, `10`

???

Je souhaite maintenant introduire une notion fondamentale en informatique : 

**La forme de base de la reproduction numérique est une suite organisée d’unités binaires.**

### Code binaire

Vers la fin des années 30, Claude Shannon démontra qu’à l’aide de « contacteurs » (interrupteurs) fermés pour « vrai » et ouverts pour « faux », il était possible d’effectuer des opérations logiques en associant le nombre 1 pour « vrai » et 0 pour « faux ».  

Ce codage de l’information est nommé **base binaire**. C’est avec ce codage que fonctionnent – encore aujourd’hui – la plupart des ordinateurs. Il consiste à utiliser deux états (représentés par les chiffres 0 et 1) pour coder les informations.

Nota : historiquement, l’aime a utilisé pour compter plusieurs systèmes différents que le système décimal : base sexadésimale (60) utilisée par les Sumériens, base duodécimale (12) utilisée par les anglo-saxons dans leur système monétaire jusqu’aux années 1960 : un round représentait vingt shilling, et un shilling douze pences

### Bit

Le terme *bit* (b avec une minuscule dans les notations) signifie « *binary digit* », c’est-à-dire 0 ou 1 en numérotation binaire. Il s’agit de la plus petite unité d’information manipulable par une machine numérique. Il est possible de représenter physiquement cette information binaire :

- par un signal électrique, magnétique ou lumineux, qui, au-delà d’un certain seuil, correspond à la valeur 1 ;
- par des aspérités géométriques dans une surface ;
- grâce à des bistables, c’est-à-dire des composants électroniques qui ont deux états d’équilibre (l’un correspond à l’état 1, l’autre à 0).

Ainsi, avec un bit, il est possible d’obtenir deux états : soit 1, soit 0. Grâce à deux bits, il est possible d’obtenir quatre états différents (2x2) ou :

| 0    | 0    |
| ---- | ---- |
| 0    | 1    |
| 1    | 0    |
| 1    | 0    |
| 1    | 1    |

--

- avec `3 bits` on peut avoir … états différents ?
- avec `8 bits` on peut avoir … états différents ?

???

- avec `3 bits` on peut avoir (2x2x2) = huit états différents
- avec `8 bits` on peut avoir (2x2x2x2) = 16  états différents ?

| Valeur binaire sur 3 bits | Valeur décimale |
| ------------------------- | --------------- |
| 000                       | 0               |
| 001                       | 1               |
| 010                       | 2               |
| 011                       | 3               |
| 100                       | 4               |
| 101                       | 5               |
| 110                       | 6               |
| 111                       | 7               |

---

count: false

## Représentation numérique

### Une suite organisée d’unités binaires

- Les ordinateurs manipulent uniquement des données de type numérique (en l’occurence sous forme binaire)

- un `bit` peut avoir la valeur `1` ou `0` (*binary digit*)

- avec `2 bits` on peut avoir quatre états différents (`2 x 2`) : `00`, `01`, `11`, `10`

- avec `3 bits` on peut avoir (`2 x 2 x 2 = 2^3 = 8`) états différents : `000`, `001`, `010`, `011`, `100`, `101`, `110`, `111`

- avec `8 bits` on peut avoir `2^8 = 256` états différents

- avec `16 bits` on peut avoir `2^16 = 65 000` états différents

- avec `32 bits` on peut avoir `2^32 = +4 millards` états différents

???

**Pour un groupe de n bits, il est possible de représenter 2^n valeurs.**  

### Octet

L’octet (en anglais *byte* ou B avec une majuscule dans les notations) est une unité d’information composée de 8 bits. Il permet par exemple de stocker un caractère, tel qu’une lettre ou un chiffre en codage ASCII. 

Ce regroupement de nombres par série de 8 permet une plus grande lisibilité. Pour un octet, le plus petit nombre est 0 (représenté par huit zéros 00000000), et le plus grand est 255 (représenté par huit chiffres « un » 11111111), ce qui représente 256 possibilités de valeurs différentes.

### KiloOctets, MégaOctets

Longtemps l’informatique s’est singularisée par l’utilisation de différentes valeurs pour les unités du système international. Ainsi beaucoup d’informaticiens ont appris que 1 kilooctet valait 1024 octets. Or, depuis décembre 1998, l’organisme international IEC a statué sur la question (http://physics.nist.gov/cuu/Units/binary.html). Voici donc les unités standardisées :

- Un kilooctet (ko ou kB) = 1000 octets
- Un Mégaoctet (Mo ou MB) = 1000 ko = 1 000 000 octets
- Un Gigaoctet (Go ou GB) = 1000 Mo = 1 000 000 000 octets
- Un Téraoctet (To) = 1000 Go = 1 000 000 000 000 octets

Attention ! certains anciens logiciels utilisent toujours la notation antérieure.

L’IEC a également défini le kilo binaire (kibi), le méga binaire (Mébi), le giga binaire (Gibi), le tera binaire (Tebi). 

- Un kibioctet (kio ou kiB) vaut 2^10 = 1024 octets
- Un Mébioctet (Mio ou MiB) vaut 2^20 = 1 048 576 octets
- Un Gibioctet (Gio ou GiB) vaut 2^30 = 1 073 741 824 octets
- Un Tébioctet (Tio ou TiB) vaut 2^40 = 1 099 511 627 776 octets

cf. http://www.commentcamarche.net/contents/95-le-codage-binaire

---

## Propriétés de la représentation numérique

- ### facile à copier

- ### reproduction sans perte (à l’∞)

- ### facile à stocker

- ### facile à transmettre

- ### facile à traiter

- ### .red[mais difficile à conserver]

???

Du fait qu’elle est constituée d’une suite organisée d’unités binaires, la représentation numérique hérite d’un certain nombre de propriétés.

---

## Les données numériques brutes

```txt
00111100011010000111010001101101011
01100001111100000110100001010001111
00011010000110010101100001011001000
01111100000110100001010000010010011
11000111010001101001011101000110110
00110010100111110010000110101001001
00010001001111001111000010111101110
10001101001011101000110110001100101
00111110000011010000101000111100001
01111011010000110010101100001011001
0000111110
```

### une suite organisée d’unités binaires, qu’on appelle aussi .red[« train de bits »]

---

## Codage et Décodage

### Pour passer d’une donnée à une information intelligible :

- ### on a besoin d’informations complémentaires sur la manière dont est codée l’information

  ### (besoin d’une .red[information de représentation])

???

La notion de codage est une notion fondamentale en informatique.

De façon générale un codage permet de passer d'une représentation des données vers une autre.

> **Codage** : Ensemble de règles définissant une correspondance biunivoque entre des informations et leur représentation par des caractères, des symboles ou des éléments de signal.
> (Jean-Alain Hernandez)

Elle implique un décodage

Attention ! *coder* n’est pas *programmer*. C’est par abus de langage que l’on parler de coder lorsque l’on écrit un programme informatique. C’est notamment lier au fait, que l’écriture des programmes informatiques manipule des symboles.

---

## Les données numériques brutes

```txt
00111100011010000111010001101101011
01100001111100000110100001010001111
00011010000110010101100001011001000
01111100000110100001010000010010011
11000111010001101001011101000110110
00110010100111110010000110101001001
00010001001111001111000010111101110
10001101001011101000110110001100101
00111110000011010000101000111100001
01111011010000110010101100001011001
0000111110
```

### .red[Indice de taille] : ceci est encodé en ASCII !

---

## Les données sont encodée en ASCII

### (= première information de représentation)

- L’[ASCII (norme ISO-646)](http://fr.wikipedia.org/wiki/American_Standard_Code_for_Information_Interchange) définit un ensemble de 128 caractères

- 33 caractères de contrôle : `DEL`, `NUL`, `EXC`

- 95 caractères typographiques : 

```
!»#$%&’()*+,-./0123456789:;<=>@
  ABCDEFGHIJKLMNOPQRSTUVWXYZ[]^_`
  abcdefghijklmnopqr stuvwxyz{|}~**
```

---

background-image: url(imagesMSL/localisation.jpg)

???

La norme ASCII définit aussi un codage (une manière de représenter les caractères dans un fichier informatique)

- les caractères occupent une taille fixe (un octet = 8 bits)
- la norme définit le lien entre combinaisons de valeurs des 7 premiers bits et les caractères
- le dernier bit est libre (usage historique du bit de parité pour lecontrôle)
- exemples :
  01100001 ou 11100001 --> a
  01100010 ou 11100010 --> b

On procède donc d’abord à la localisation des unités.

---

## Les unités décodées

```bash
<html>CR.LF<head>CR.LF.TAB<title>SAE
</title>CR.LF</head>CR.LF<body>
CR. LF.TAB<p style=»color:#ff0000»>
CR.L F.TAB.TAB.Bonjour.CR.LF.TAB</p>CR.L F</body>CR.LF</html>
```

---

count: false

## Les unités décodées

```html
<html>CR.LF<head>CR.LF.TAB<title>SAE</title>CR.LF
</head>CR.LF<body>CR. LF.TAB<p style=»color:#ff0000»>
CR.L F.TAB.TAB.Bonjour.CR.LF.TAB</p>CR.L F</body>CR.LF</html>
```


--

#### Les données sont encodée en HTML (= deuxième information de représentation)

- Le texte ASCII respecte la syntaxe HTML
- HTML (Standard W3C) définit un ensemble de conventions (noms et signification de balises, etc.) dans une syntaxe elle même définie en SGML (norme ISO-8879:1986)

#### Le contenu des attributs style respecte la syntaxe CSS (= troisième information de représentation)

- CSS (standard W3C) définit un ensemble de conventions formelles pour exprimer des propriétés de mise en page
- CSS utilise pour exprimer certaines valeurs des encodages spécifiques : URL pour les noms de fichiers, RVB pour les couleurs, etc.

???

Pour passer de la donnée numérique à un contenu d’informations échangeable, il a fallut ajouter des informations de représentation

- Codage des caractères en ASCII
- Texte dans une syntaxe HTML
- Aspects de mise en page dans une syntaxe CSS
- Codage des couleurs en RVB

---

## La question de la compatibilité

```bash
01010010 01000101 01000110 01000110 00110000 00000000
00000001 00000000 01010111 01000001 01010110 01000101
00010000 00000000 00000000 00000000 00000001 00000000
00000001 00000000 00010001 00101011 00000000 00000000
00010001 00101011 00000000 00000000 10000000 10000000
10000010 10000100 10001000 10001110

```

--

count: false

#### rien ne vous permet a priori de le distinguer de l’exemple précédent

.red[(besoin d’une information de représentation de représentation)]

--

count: false

#### Or, ceci est un extrait de code d’une vidéo au format `WAV`

---

## Informations de représentation

- Unified Digital Format Registry (UDFR), a semantic registry for digital preservation (2010-2012) http://www.udfr.org
- UK National Archives’s [PRONOM](http://www.nationalarchives.gov.uk/PRONOM)
- http://digital-preservation.github.io
- Media Types https://www.iana.org/assignments/media-types/media-types.xhtml
- https://www.nist.gov/software-quality-group/national-software-reference-library-nsrl
- http://digitalpreservation.gov
- http://jhove.openpreservation.org
- https://facile.cines.fr
- http://www.loc.gov/standards/premis/

???

Besoin d’informations de représentation

---

## Obsolescence technique

![image](imagesMSL/preservationObsolescence.png)

???

e

---

## Menaces physiques

![image](imagesMSL/preservation.png)

???

e

---

## L’archivage pérenne des docuemnts numériques

Une opération active, conçue sur le très long terme (30 ans et au-delà) : archivage ≠ archivage pérenne | archivage pérenne ≠ sauvegarde

Une triple fonction

- conserver le document
- le rendre accessible
- en préserver l’intelligibilité

https://www.cines.fr/wp-content/uploads/2013/12/Archivage_perenne_Gazette20.pdf

???

Archivage ≠ de l’archivage pérenne.

Archivage pérenne ≠ sauvegarde : 

- pas un service HSM hierarchical storage manager où l’on migre des fichiers sur bande pour faire de la place sur les disques
- pas non plus une utilime étape deu stockage des donénes avant leur oubli ou leur perte définitive.

Une opération active, conçue sur le très long terme (30 ans et au-delà). Il s’agit de conserver un accès au document, mais aussi son intelligibilité. Problème du stockage informatique. Sécurisation contre les pertes accidentelles. Prise en compte des risques d’obsolescence qui pourraient rendre le contenu illisible.

L’obsolescence terchnologique est un phénomène inéluctable. L’archivage pérenne vise à apporter des solutions technologiques et organisationnelles pour garantir la conservation, l’accès et l’intelligibilité des documents.

Prendre en compte :

- l’obsolescence technique
- la dégradation des supports

---

## L’importance des métadonnées

- identification de toutes les métadonnées qui doivent accompagner un document numérique

???

Afin de permettre la pérennisation à long terme de l’information numérique, l’identification de toutes les métadonnées qui devront accompagner un document numérique est un travail difficile mais crucial car elle va directement conditionner la qualité du service d’archivage et l’accès future au document.

Peu d’expérience à long terme.

- Métadonnées de référence Dublin Core qui constituent un noyau généraliste de métadonnées descriptives. 
- Il convient d’y ajouter des métadonénes plus techniques et spécialisées dans la pérennisation.

Approche de type gestion des risques. 



---

## Le Modèle OAIS

![image](imagesMSL/oaisModel.gif)

???

> L'**Open Archival Information System** ou **OAIS** (Système ouvert d'archivage d'information) est un modèle conceptuel destiné à la gestion, à l'[archivage](https://fr.wikipedia.org/wiki/Archivage) et à la préservation à [long terme](https://fr.wikipedia.org/wiki/Long_terme) de [documents numériques](https://fr.wikipedia.org/wiki/Document_%C3%A9lectronique). La mise au point de l'OAIS a été pilotée par le [Consultative Committee for Space Data Systems](https://fr.wikipedia.org/wiki/Consultative_Committee_for_Space_Data_Systems). L'OAIS est enregistré comme [norme ISO](https://fr.wikipedia.org/wiki/Liste_de_normes_ISO) sous la référence 14721:2012.
>
> Le modèle OAIS constitue une référence décrivant dans les grandes lignes les fonctions, les responsabilités et l’organisation d’un système qui voudrait préserver de l’information, en particulier des [données numériques](https://fr.wikipedia.org/wiki/Document_%C3%A9lectronique), sur le long terme, pour en garantir l'accès à une communauté d'utilisateurs identifiés. Le long terme est défini comme suffisamment long pour être soumis à l’impact des évolutions technologiques.
>
> wikipédia

La perte des données numériques de plusieurs des premières missions spatiales ayant entraîné une forte prise de conscience quant aux enjeux de la pérennisation de l’information numérique

*Consultative Committee on Space Data Systems* (CCSDS, 2012) dans les années 1990 est devenu une norme ISO (ISO14721) en 2003, et fut révisé en 2012. Traduction en français disponible depuis le printemps 2005.

Le modèle OAIS est venu standardiser les pratiques en proposant un vocabulaire contrôlé, un modèle de données, six fonctions essentielles que doit remplir un bon système de préservation numérique et six responsabilités qui incombent à ces systèmes et leurs administrateurs

Le modèle OAIS identifie quatre rôles dans un système d’archivage, trois externes et un interne.

- acteur interne, l’archive autrement dit l’opérateur du système d’archivage
- le management qui assume les décision politiques
- les producteurs les personnes ou les organismes qui fournissent les objets à archiver
- les utilisateurs

Archives SIP submission information package

Une fois archivés deviennent les AIP archival information package

DIP dissemination information package.

Fonctions d’archivage

- Entrées
- plannifaction de la pérennisation, veille et planification
- gestion des données, prend en charge la tenue à jour de toutes les informations
- stockage assure la conservation phyisque des objets archivés
- Administration, coordination du système
- Accès

Rafraîchissmenet

Duplication

Ré-empaquetage

Transformations



Autrs normels

PAIMAS Producer-Archive Interface Methodology Abstract Standard CCSDS

Norma AFNOR NF 21-013, GED et gestion électronique des documents.

ISO 15489 Records Management et MoReq (Europe)



---

## Initiatives Canadiennes de préservation/conservation

### Groupe de travail sur la préservation numérique

En 2016, l’ABRC a réuni différents membres des bibliothèques et des archives pour former un [Groupe de travail sur la préservation numérique (GTPN)](https://www.carl-abrc.ca/fr/faire-avancer-la-recherche/conservation-numerique/).

### Borealis

https://borealisdata.ca

- Anciennement [Scholars Portal](https://scholarsportal.info), depuis 2013
- Intégration du BCI en 2022 et changement de nom

???

[CARL/ABRC](https://www.carl-abrc.ca), l’association des bibliothèques de recherches au Canada regroupe 29 des plus grandes bibliothèques universitaires du pays et deux établissements fédéraux.

L’organisation a joué un rôle clé dans les discussions relatives à la préservation des archives du Canada qu’elles soient imprimées ou numériques. En 2022, elle a participé à la création de [Nord](https://northnordsharedprint.ca/fr/acceuil/), un Réseau canadien de conservation partagée des documents imprimés qui faisait suite au [Groupe de travail sur la stratégie canadienne de préservation des collectiosn collectives d’imprimés](http://www.bac-lac.gc.ca/fra/services/collections-imprimees-partagees/Pages/collections-imprimees-partagees.aspx) de 2018.

[Leviathan du Nord](https://www.carl-abrc.ca/uploads/pdfs/Leviathan_North_Report_FINAL.pdf) 2014.

Plusieurs initiatives locales : cf. https://www.carl-abrc.ca/fr/faire-avancer-la-recherche/collections-de-recherche/initiatives-de-conservation/

### Groupe de travail sur la préservation numérique

En 2016, l’ABRC a réuni différents membres des bibliothèques et des archives pour former un [Groupe de travail sur la préservation numérique](https://www.carl-abrc.ca/fr/faire-avancer-la-recherche/conservation-numerique/). Ce groupe réunit notamment plusieurs bibliothèqies universitaires, centres d’archives ou organismes régionaux tels que Canadiana.org, Bibliothèque et archives Canada, ou BAnQ) pour travailler à l’intendance à long terme des contenus nuémriques :

- étude des capacités actuelles du pays
- [Coalition canadienne pour l’archivage sur le Web](https://www.carl-abrc.ca/fr/faire-avancer-la-recherche/conservation-numerique/ccaw/) (CCAW) issue du GTCN réunit des personnes travaillant sur la préservation du contenu web

> Ce groupe travaille à l’intendance à long terme du dossier académique numérique canadien et du patrimoine documentaire multiformat et soutient le mandat spécifique du Comité sur l’avancement de la recherche de l’ABRC afin de préserver l’ensemble de la documentation savante et le patrimoine documentaire sous toutes ses formes au Canada. Son travail comprend l’évaluation de la capacité, les ressources disponibles et les possibilités de financement présents dans le milieu canadien de la recherche en matière de préservation numérique, et l’identification et la promotion des approches, des normes, des pratiques et des technologies pertinentes, assurant la liaison avec les efforts similaires au niveau international.

Un des efforts liés à ce groupe est la [Coalition canadienne de l’archivage Web](https://www.carl-abrc.ca/fr/faire-avancer-la-recherche/conservation-numerique/ccaw/).

Ce groupe a aussi organisé un forum ouvert d’une journée en novembre 2018 sur la préservation numérique au Canada, [@Risk North 2 : Collections numériques en péril](https://www.carl-abrc.ca/fr/mini-site-page/risk-north-2-collections-numeriques/).

### Scholars Protal et Borealis

Scholars Portal Trusted Digital Repository https://www.ocul.on.ca/node/97

- Open Archival Information System
- Trustworthy Repositories Audit & Certification (TRAC) checklist 
- ISO 16363 standard (Audit and Certification of Trustworthy Digital Repositories), depuis 2013

Borealis 

> Borealis, le dépôt Dataverse canadien, est un dépôt canadien de données de recherche bilingue, multidisciplinaire et sécurisé, soutenu par des bibliothèques universitaires et des établissements de recherche de partout au Canada. Borealis permet la découverte, la gestion, le partage et la préservation des données de recherche canadiennes. 

Cet entrepôt utilise le logiciel [Dataverse](https://dataverse.org) qui est un logiciel libre développé par l’Institute of Quantitative Social Science (IQSS)  de l’Université Harvard et une communauté de développement mondiale.

### Divers (pour mémoire)

Service de conservation du Conseil des bibliothèques universitaires des Prairies et du Pacifique

- COPPUL (2018). « What is the COPPUL DPN ? », \*Council of Prairie and Pacific University Libraries\*. https://coppul.ca/programs/coppul-dpn/about

ARTEFACTUAL SYSTEMS INC. (2018). Archivematica. https://www.archivematica.org depuis 2015

### Musées

Des initiatives canadiennes qui pourraient servir de modèle collaboratif pour la communauté muséale québécoise. Utilisation de plateforme infonuagique, association fournissant expertise et soutien technique agissant comme consortium pour assurer et sensibiliser à l’intendance numérique. Adhésion volontaire à des servcies de traitement et de stockage. Solutions flexibles pour des institutions de taille diverse.

> L’utilisation de plus en plus courante de systèmes de conservation libres et gratuits tels que Archivematica représente également une forme de collaboration couronnée de succès. Basé sur une vaste gamme de standards établis tels que OAIS, PREMIS et Dublin Core, Archivematica rejoint une grande variété d’utilisateurs. En plus de mettre à disposition de cette large communauté la documentation et l’infrastructure de développement du logiciel aux fins d’études, d’adaptation et de redistributions, les développeurs encouragent les usagers à partager leurs contributions et modifications afin d’offrir une plateforme en constante évolution (Artefactual Systems Inc., 2018). L’entreprise canadienne à l’origine de ce logiciel favorise dès lors une collaboration qui contribue à améliorer la normalisation et les outils de préservation numérique disponibles. En effet, « […] si de nombreuses institutions utilisent un même logiciel libre, il est plus facile d’améliorer le système d’origine grâce à des suggestions provenant de sources multiples. La difficulté est de se concentrer sur la mise en œuvre des normes existantes et de résister à la tentation d’en élaborer de nouvelles. » (CAC, 2015 : 125)

---

## L’exemple français

### Système de Préservation et d'Archivage Réparti SPAR

https://www.bnf.fr/fr/spar-systeme-de-preservation-et-darchivage-reparti

Bnf et Ministère de la culture

### Centre Informatique National de l’Enseignement Supérieur CINES

https://www.cines.fr/archivage/

Enseignement supérieur

### Vitam

SIAF, Archives des affaires étrangères

https://francearchives.gouv.fr/fr/article/162808225

???

### Système de Préservation et d'Archivage Réparti SPAR

https://www.bnf.fr/fr/spar-systeme-de-preservation-et-darchivage-reparti

Lancé en 2010, et continuellement enrichi de nouvelles collections et fonctionnalités.

> Au-delà d’un simple stockage sécurisé, le système SPAR cherche à garantir la **préservation** des documents numériques : à faire en sorte que l’information reste lisible, compréhensible et réutilisable sur le long terme, même si l’environnement technique et humain dans lequel ces documents ont été produits change. Comme il est souvent difficile de réparer des documents numériques après dégradation ou de les relire après disparition des matériels et logiciels d’époque, l’effort porte sur les opérations préventives de veille et de migration.
>
> SPAR contribue également à la réalisation des opérations d’**archivage** numérique : gestion documentaire, suivi de l’authenticité des documents à des fins de preuve, garantie de la sécurité du système, etc. Enfin SPAR est dit «réparti» car il permet la gestion de plusieurs copies des documents, sur plusieurs sites, afin de se prémunir contre les pertes et destructions.

Conçu selon les principes de l’OAIS

### Centre Informatique National de l’Enseignement Supérieur CINES

https://www.cines.fr/archivage/

Le CINES a reçu en 2004 le mandat du ministère de l’enseignement supérieur et la recherche pour devenir l’opérateur pour l’archivage des données et documents numériques produits par la communauté de l’Enseignement supérieur et de la recherche. Il propose des solutions d’archivage numérique à moyen et long terme mutualisées et personnalisables pour les données scientifiques, les archives publiques et les ressources des bibliothèques et centres de documentation.

https://www.cines.fr/wp-content/uploads/2013/12/Archivage_perenne_Gazette20.pdf

### Programme Vitam

https://www.programmevitam.fr

PAC et VITAM

---

## Digitization and Digital Preservation

- digital preservation Policy Framework Development Guidelines
- concepts for developing Digital preservation policies (ancien mais toujours valable)
- digital preservation decisition tree model to establish whether a digital ressource should be preserved (dérivé British lib? mais beaucoup simplifié)

???

Enquête parmi identifié que pas de planification préservation. Parfois GitHub.

Développement de standard de préservation et bonne pratiques pour les institutions patrimoniales.

- digitization and digital preservation discussion group
- national heritage digitization strategy

Formation en face-à-face CCI Digital preservation workshop. Lectures dans les institutions patrimoniales.

Digital preservation Toolkit : workflow, bonnes pratiques, guidelines. Encore besoin de le promouvoir. Cas d’études. Focalisation sur les petites institutions car beaucoup besoin d’agir à ce niveau.

Ressources pour Digital Asset Surveys

- template pour inventaire de préservation numérique
- cas d’étude du musée d’histoire du Canada

Ressources pour Policy Development
Projet du Getty? mais difficilement applicable pour des petites institutions

- digital preservation Policy Framework Development Guidelines
- concepts for developing Digital preservation policies (ancien mais toujours valable)
- digital preservation decisition tree model to establish whether a digital ressource should be preserved (dérivé British lib? mais beaucoup simplifié)

Founiture de documents

- digital preservation plan framework for museums
- digital preservation best practices for museums
- interpares 2 creator Guidelines
- interPares 2 Preserver Guidelins
- New: document pour petits musées
- bientôt recommandations sur les formats de fichiers (pour NHDS)

Cas d’usage, car toolkit pour petites organisations. Si grandes organisation différent. Sans doute besoin de cas différents comme modèles. Petit musée, musée devenu important.

Ressources pour la numérsiation. Révision des documents de recommandation et bonnes pratiques. Documentation facile d’accès et ciblée sur les petites institutions.

erm.bieman@canada.ca

Discussion

Va beaucoup mieux pour la numérisation mais problème de financement pour la préservation. Dans les politiques essaye de focaliser sur qui doit être impliqué. Policy qui est surtout un ensemble d’outil de gestion du changement pour convaincre organisation. Mais clairement, l’argent doit venir de quelque part.

En introduction évoquait besoin de lier la documentation à la diffusion des images. Savoir si dans les politiques cette question mise en avant.

Canadiana, certaines bibliothèques, NSTS au niveau national. Mais pas vraiment d’initiative de ce type.

---

## Politiques Canadiennes

- 2016 « Boîte à outils de la préservation numérique », Gouvernement du Canada. <https://www.canada.ca/fr/reseau-information-patrimoine/services/preservation-numerique/boite-outils.html>
- Réseau canadien d’information sur le patrimoine (RCIP). « Lignes directrices sur l’élaboration d’un cadre stratégique pour la préservation numérique ». Canadian Heritage Information Network, 28 août 2017. https://www.canada.ca/fr/reseau-information-patrimoine/services/preservation-numerique/lignes-directrices-elaboration-cadre-strategique.html.
- 2011 « Sondage sur la préservation numérique : résultats préliminaires de 2011 », Gouvernement du Canada. <https://www.canada.ca/fr/reseau-information-patrimoine/services/preservation-numerique/sondage-resultats-preliminaires-2011.html>
- 2006 « Anne Kenney et Nancy McGovern sur les dix bonnes raisons pour envisager la préservation numérique », Gouvernement du Canada. <https://www.canada.ca/fr/reseau-information-patrimoine/services/preservation-numerique/dix-raisons-envisager-preservation-numerique.html>
- « Gestion des contenus numériques et les musées – Introduction », Gouvernement du Canada. <https://www.canada.ca/fr/reseau-information-patrimoine/services/systemes-gestion-collections/gestion-contenus-numeriques-musees.html>
- « Préservation numérique », Gouvernement du Canada. <https://www.canada.ca/fr/reseau-information-patrimoine/services/preservation-numerique.html>

???

Conseil des bibliothèques universitaires des Prairies et du Pacifique (COPPUL DPN). En service depuis 2015, ce réseau spécialisé propose à ses membres une foule de services relatifs à la pérennisation de leurs contenus numériques par le biais d’une plateforme infonuagique.

COPPUL (2018). « What is the COPPUL DPN ? », Council of Prairie and Pacific University Libraries.* [https://coppul.ca/programs/coppul-dpn/about]

Archivematica par Artefactual Systems Inc., 2018. L’entreprise canadienne à l’origine de ce logiciel favorise dès lors une collaboration qui contribue à améliorer la normalisation et les outils de préservation numérique disponibles. En effet, « […] si de nombreuses institutions utilisent un même logiciel libre, il est plus facile d’améliorer le système d’origine grâce à des suggestions provenant de sources multiples. La difficulté est de se concentrer sur la mise en œuvre des normes existantes et de résister à la tentation d’en élaborer de nouvelles. » (CAC, 2015 : 125)

ARTEFACTUAL SYSTEMS INC. (2018). « Home », Archivematica. [https://www.archivematica.org/fr/]

Un document publié par le Conseil des académies canadiennes en 2015 mentionne d'ailleurs que les initiatives nationales dans le domaine sont complètement en retard et inefficaces comparativement aux initiatives de la Grande-Bretagne, de l'Union européenne et de l'Australie. (<http://sciencepourlepublic.ca/uploads/fr/assessments%20and%20publications%20and%20news%20releases/memory/CofCA_14-377_MemoryInstitutions_WEB_F.PDF>) 

Direction Interministérielle du Numérique et du Système d’Information et de Communication de l’État, Référentiel Général d’Interopérabilité. Standardiser, s’aligner et se focaliser pour échanger efficacement Version 2.0, December, 2015. <http://references.modernisation.gouv.fr/interoperabilite> (accessed May 12, 2016). 

<http://www.ledevoir.com/societe/science-et-technologie/468593/centre-canadien-d-architecture-sauver-les-fichiers-d-hier-et-d-aujourd-hui>

<http://www.ledevoir.com/societe/science-et-technologie/468595/sauvegarde-des-donnees-quand-le-numerique-nous-fait-perdre-la-memoire>

Un Rapport de Ithaka pour la gestion de contenus numériques en milieu culturel : Pickle, Sarah, and Nancy L Maron. January 29, 2013. <http://www.sr.ithaka.org/publications/sustaining-our-digital-future>. 

Fuentes Hashimoto, Lourdes and Pierre Marcotte. "Back to basics : et si on relisait Pérotin ?."<http://archivesonline.wordpress.com/2011/10/12/back-to-basics-relire-perotin/> (accessed August 11, 2013).

Dunant Gonzenbach, Anouk. "Les mains dans le cambouis et la théorie des 3 âges." <http://present-hieretdemain.tumblr.com/post/22661817291/les-mains-dans-le-cambouis-et-la-theorie-des-3-ages> (accessed August 11, 2013).

Brégier, Frédéric. "SAE, OAIS, les 3 âges : vus par un informaticien." <http://archiverleternite.blogspot.fr/2013/07/sae-oais-les-3-ages-vus-par-un.html?utm_source=dlvr.it&utm_medium=twitter>. 

Un document du Ministère de la Culture et de la Communication sur le sujet de 2008 Conservation à long terme des documents numérisés,<http://www.culture.gouv.fr/culture/mrt/numerisation/fr/technique/documents/conservation.pdf>.

---

## Normes et standards

[PREMIS Data Dictionary for Preservation Metadata](https://www.loc.gov/standards/premis/)

???

> The PREMIS Data Dictionary for Preservation Metadata is the international standard for metadata to support the preservation of digital objects and ensure their long-term usability. Developed by an international team of experts, PREMIS is implemented in digital preservation projects around the world, and support for PREMIS is incorporated into a number of commercial and open-source digital preservation tools and systems. The PREMIS Editorial Committee coordinates revisions and implementation of the standard, which consists of the Data Dictionary, an XML schema, and supporting documentation.

---

## Plusieurs stratégies de conservation possibles

#### stockage éphémère

#### migration d’un support à l’autre

#### émulation

#### réinterprétation de l’œuvre

???

« Are your born digital ? »
Pour Bernhard Serexhe, telle pourrait être dans un avenir proche la question cruciale que l’on pourrait poser à propos de la conservation de l’art de notre temps et sa mise à disposition pour les générations futures.

ZKM Centre d’art et de Technologie des Médias Karlsruhe initié un projet de recherches _digital art conservation_.
Comprendre les conditions actuelles de conservation – ou de non conservation - de l’art numérique présent dans les collections, et proposer et tester des stratégies en vue d’une conservation ultérieure.

À l’instar du ZKM, d’autres institutions à travers le monde, telles que la Tate Modern, ou encore le Whitney Museum of Art se sont également engagées sur des projets ayant pour objectif d’améliorer et de trouver des solutions adaptées à la conservation des œuvres d’art nativement numérique.

Aux possibilités potentiellement illimités offertes par le numérique, réponde autant de problèmes spécifiques de conservation pour les institutions patrimoniales.

Ces problématiques rejoignent en partie la question plus générale de la pérennisation de l’information numérique à long terme. Mais elle n’est pas réductible à cette seule pérennisation. En effet, il s’agira ici de prendre en compte certains aspects spécifiques de l’œuvre d’art numérique dont on a vu qu’ils pouvaient avoir une grande importance cruciale pour la compréhension et la réception de certaines réalisations.

La conservation de l’art numérique interroge aussi la conservation proprement dite en obligeant à envisager de manière différente des questions canoniques comme celles de la sacro-sainte « authenticité ». Désir légitime de conserver cette « authenticité » mais ne doit pas du même coup risquer de causer la perte de l’œuvre sous prétexte de défaillance technique.

Par ailleurs, il est relativement acquis que l’art numérique dispose très souvent d’un caractère performatif, et partant, éphémère. Pour conserver ses fonctionnalités techniques, son comportement donc, il convient parfois mieux d’en adapter constamment la technique à la « situation d’exécution » donnée.

Pour autant, ne pas renoncer à définir clairement l’origine de l’œuvre d’art et sa classification, ni non plus « améliorer » techniquement ou esthétiquement les œuvres. Doivent conserver aussi longtemps et fidèlement que possible leurs caractère, comportement et esthétique d’origine ; elles doivent pouvoir témoigner de l’époque et des circonstances de leur création.

Production artistique concernée par la nouveauté et peu préoccupée pendant longtemps par les paradigmes classiques du monde de l’art tels que l’authenticité, la conservation, etc. Refus de certains artistes d’aborder le marché de l’art, ou insularisation de la pratique qui n’a pas forcément contribué à la conservation des œuvres.

Seulement récemment que plusieurs grandes institutions patrimoniales et culturelles s’engagent dans la collecte, la conservation mais aussi l’exposition de ce type d’œuvres.

- Problèmes d’exposition particulier. Comment représenter sans dénaturer (cf. ce qu’avait vu à propos de la Documenta X).
- Comment recréer installations numériques lorsque technologies devenues obsolètes ? Aspect performatif de l’art numérique, qui permet de s’interroger sur le fait même que cela ait du sens.
- Quid des forums et autres formes présentent sur le web.

Nouveauté perpétuelle ?
Amnésie continuelle ?

Dimension éphémère des réalisations. Valeur heuristique de l’exploration du medium irrémédiablement perdue.

Ainsi les production de l’art numérique appellent probablement de nouveaux modes de conservation, mais aussi de collectionnement qui rende justice aux intentions initiales des créateurs.

Approche spécifique du média, et importance de la conservation de l’œuvre dans son état original pour pleinement témoigner des conditions de sa conception et de sa réalisation.

- Mais qu’est-ce qu’un original à l’ère du numérique ?
- Qu’en est-il de la matérialité d’une œuvre numérique ?
- Quels sont les éléments pertinents qu’il peut être intéressant de chercher à conserver ?

– **Le stockage** apparaît alors comme la solution la plus classique, mais aussi la plus conservatrice – la stratégie par défaut pour la plupart des musées – qui consiste à entreposer à la fois l’équipement spécialisé et à archiver les fichiers sur un support numérique. Le principal désavantage de cette première stratégie est que l’œuvre viendra à disparaître ou périra lorsque ces matériaux désuets et ces données obsolètes cesseront de fonctionner.

– **La migration** implique au contraire la mise à niveau de l’équipement et du matériel source. Il y aura migration lorsque l’on choisira de remplacer ce matériel et de convertir dans un nouveau format un fichier informatique (rendu illisible par l’obsolescence de la technique originelle) pour l’enregistrer dans une version plus récente. Le désavantage majeur de la migration est que l’apparence de l’œuvre originelle peut significativement changer lors d’une mutation importante des systèmes et des interfaces technologiques. Car en effet la migration peut avoir pour conséquence le changement d’apparence d’une pièce, du fait notamment de la disparition de certaines fonctionnalités d’une version à l’autre d’un logiciel.

– **L’émulation**, consiste à recréer l’apparence d’une œuvre mais à partir d’un code source différent. Il s’agit alors d’un traitement plus complexe qui consiste à adapter et à faire fonctionner les codes informatiques originaux sur des ordinateurs de générations ultérieures aux codes eux-mêmes.
En installant les différentes couches logicielles qui ont été conservées, il devient possible d’exécuter à nouveau certains fichiers, originaux ou modifiés, afin de réactualiser l’œuvre. Mais si l’émulation logicielle est une technique éprouvée et relativement stable pour les dispositifs autonomes, qui ne dépendent pas de la labilité du réseau, elle s’avère moins évidente dans le cas du Net art. En effet, les paramètres qui déterminent le bon fonctionnement d’une œuvre Net art sont pluriels et très fragiles

– **La ré-interprétation**, stratégie la plus radicale, consiste à re-interpréter l’œuvre lors de chacune de ses actualisations. Il s’agit toujours de recréer, grâce aux données recueillies par le musée, suite aux entretiens et questionnaires avec l’artiste ou avec les ayants droit, ainsi qu’avec des historiens de l’art et des informaticiens, une œuvre fidèle à l’intention de l’artiste mais qui peut s’avérer très différente de l’original. Cette solution est sans doute la plus risquée mais c’est aussi celle qui permet au musée de changer de rôle face aux œuvres. Comme l’énonce Jon Ippolito, « aussi excentrique que l’idée puisse paraître aux pratiques traditionnelles de collection, [cette vision de la conservation] offre une alternative pour ceux dont la conception de leur œuvre va au-delà de sa manifestation dans une forme particulière. Et elle nous aide à imaginer le musée comme un incubateur pour des œuvres d’art vivantes, changeantes, plutôt que comme un mausolée pour des œuvres mortes. »

---

background-image: url(images/digitalConservation.jpg)

[http://www.digitalartconservation.org](http://www.digitalartconservation.org)

???

## Digital Conservation ZKM

### Projet initié par ZKM et conduit de 2010-2012 et dédié à rechercher des stratégies pour la conservation de l’art numérique.

Le projet s’est principalement concentré sur les œuvres créées avec des technologies numériques et la programmation par ordinateur

Conduit en collaboration avec autres institutions région rhénane.
Perpective pratique.

---

## La notion de "Média variables"

http://www.fondation-langlois.org/html/f/page.php?NumPage=200

http://www.variablemedia.net

### DOCAM

http://www.docam.ca

### Update or Die

https://phi-centre.com/en/event/update-or-die/

???

### Une approche concertée

Engager un dialogue entre l’artiste et l’institution pour mieux connaître les caractéristiques techniques de l’œuvre, afin d’en prévoir les évolutions et de définir la perte acceptable.

Notion de _Média variables_
initié par l’artiste **Jon Ippolito**, conservateur au musée Guggenheim de New York l’œuvre d’art comme un ensemble d’instructions susceptibles d’être ré- interprétées et adaptées suivant l’évolution technique et culturelle

L’artiste est donc moins invité à spécifier l’état idéal de présentation de son œuvre, qu’à décrire finement ces états passés et futurs, en tenant compte d’une part des variations (déjà connues) qui ont marquées chaque actualisation et ré-exposition de l’œuvre, et en projetant d’autre part ces variations à venir en choisissant un devin possible de l’œuvre parmi les quatre stratégies de conservations précitées.

Approche qui permet l’ouverture des musées aux logiciels artistiques du software art, aux jeux informatiques et aux dispositifs en réseau.
Et fichiers de documentation.

Accessibilité technique

### Variable Media Initiative

http://www.guggenheim.org/variablemedia

The Guggenheim's approach to preserving online art, called the Variable Media Initiative (http://www.guggenheim.org/variablemedia), prepares for the obsolescence of ephemeral technology by encouraging artists to envision the possible acceptable forms their work might take in future mediums.

The preservation of intangible and often collaborative works dispersed across a global network requires the museum to forego its expertise with traditional artistic media and develop a facility with 21st-century tools and technology. However, preserving Internet works of art requires more than simply archiving Web files on a server or CD-ROM. Along with the digital files corresponding to each piece, the Guggenheim compiles data on how the artwork is to be translated into new mediums once its original hardware and software are obsolete. To prepare for such future re-creations, the Guggenheim has created a variable media endowment, the interest of which is earmarked for future costs of data migration, emulation, and reprogramming.

https://web-beta.archive.org/web/20110429032301/http://www.guggenheim.org/new-york/press-room/releases/press-release-archive/2002/668-february-18-internet-art-commissions

---

## Bibliographie

- Rieger, Oya Y., Roger C. Schonfeld, et Liam Sweeney. « The Effectiveness and Durability of Digital Preservation and Curation Systems ». Research report. Ithaka S+R, 19 juillet 2022. https://sr.ithaka.org/publications/the-effectiveness-and-durability-of-digital-preservation-and-curation-systems/.
- *Special Issue Introduction: Managing Digital Assets in US Museums*. RLG DigiNews 10, n° 6, 2006. https://worldcat.org/arcviewer/1/OCC/2007/07/10/0000068924/viewer/file1.html.

---

## Bibliographie

- Ramón Reichert, Annika Richterich, Pablo Abend, Mathias Fuchs, Karin Wenz (eds.). _Digital Culture & Society_ Vol. 1, Issue 1 – Digital Material/ism, September 2015. ISBN 978-3-8376-3153-1
- Laforet, Anne. _Le Net Art au Musée : Stratégies de Conservation des œuvres en ligne_. Paris : Questions théoriques, 2011.
- Serexhe, Bernd (dir.). _Conservation de l’art numérique, Théorie et pratique. Le projet Digital Art Conservation_. Karlsruhe; Vienne : ZKM ; Ambra V, 2013.
- [http://notepad.benfinoradin.info](http://notepad.benfinoradin.info)
- Fourmentraux, Jean-Paul. "Art Et Médias Variables. Préserver, Exposer Et Pratiquer Les Œuvres Numériques." Les cahiers du numérique 8, no. 4 (2012): doi:10.3166/lcn.8.4.33-52.
- Kirschenbaum, Matthew G., Erika L. Farr, Kari M. Kraus, Naomi Nelson, Catherine Peters, Gabriela Redwine, and Doug Reside. "Digital Materiality: Preserving Access to Computers As Complete Environments." iPres (2009). http://escholarship.org/uc/item/7d3465vg.pdf. 

---

background-image: url(imagesMSL/metadataNoFuture.png)

---

background-image: url(imagesMSL/clouds768_loop.gif)



???

## Conclusion

Au sein de la fonction centrale de la régie des œuvres, l’inventaire et le traitement informatique des collections occupe une place de plus en plus centrale au sein des musées.

C’est sans doute un des domaines de l’activité muséale qui a connu la plus forte transformation avec l’irruption de l’ordinateur et des bases de données. Aujourd’hui, ces applications sont devenues cruciales non seulement pour mettre à disposition du public le catalogue des collections sur le web mais aussi pour la production de contenus numériques élaborés.

Au cours du semestre, nous avons passé en revue le cadre normatif de la production muséale au niveau national et international. Nous avons envisagé à la fois des questions techniques et pratiques liés à la représentation de l’information muséale sous forme informatique et des questions conceptuelles. Plus généralement, nous avons introduit des notions d’interopérabilité et approfondi la question du web sémantique et du web de données. Et j’ai introduit plusieurs éléments sur l’utilisation des logiciels de gestion des collections.

Comme vous l’avez compris, je n’ai pas souhaité vous former à un logiciel en particulier. D’abord parce que les produits installés varient d’une institution à l’autre, mais surtout parce qu’il n’existe actuellement pas de solution miracle. Ce que j’ai voulu faire c’était vous former aux questions intellectuelles relatives à la description muséale.

La place de plus importante qu’occupe l’informatisation à tous les niveaux de l’institution fait en effet émerger de nouveaux métiers. Je crois vous avoir suffisamment montré à quel point ces fonctions réclament un savoir et une expertise de type muséale et pouvaient difficilement être confiés à de simple informaticiens.

Un savoir muséal spécifique à mobiliser

- production des normes métiers
- intégration et agrégation de données
- conception des systèmes d’information
- politique de valorisation numérique
- production d’expositions virtuelles.

