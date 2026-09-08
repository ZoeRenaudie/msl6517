title: CIECO
description: emchateau UdeM
theme: presentation/theme/remark-dark-em.css
name: inverse
layout: true
class: inverse

---

name: index

class: center middle

# Web sémantique et ontologies dans le domaine patrimonial

### 17 octobre 2021 | Emmanuel Château

---

class: inverse, center, middle

# Introduction

???

L’hétérogénéité de l’information muséale

Les technologies du web sémantique et l’approche du web de données liées désignent une combinaison de techniques d’outils et de standards qui permettent de transformer le world wide web d’un web de documents à un web de données. Lorsque cette approche est appliquée au monde des bibliothèques, des archives et des musées, les données liées transforment la manière dont nous pouvons découvrir, analyser, et visualiser les contenus culturels et scientifiques.

Les données ouvertes et liées (Linked Open Data LOD) permettent aux institutions patrimoniales et culturelles de publier et partager des informations sur leur collections en ouvrant d’infinies possibilités de réutilisations et d’enrichissements et afin d’augmenter leur visibilité.

Cependant, les acteurs du monde culturels sont confrontés à plusieurs enjeux dans l’appropriation de ces technologies :

- bien sûr, l’adoption de ces technologies et de ces standards nécessite des compétences techniques particulières. Pour autant, ce n’est pas le seul enjeu pour les institutions ou les acteurs du secteur culturel.
- En effet, partager les données des collections suppose l’adoption de politiques d’ouverture de données adaptées
- cette démarche présente également des enjeux relatifs à l’autorité des institutions. Dans un contexte distribué, il y a un changement d’échelle qui n’est pas sans impact sur les collection.

Plusieurs enjeux pour les institutions

- catalogues et identité des musées
- changement d’échelle

LODLAM Linked Open Data Libraries, Archives and Museums

Le rêve de l’historien de l’art rencontre ce que font actuellement les musées

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

---

## Données 5 étoiles

- ★ make your stuff available on the Web (whatever format) under an open license
- ★★ make it available as structured data (e.g., Excel instead of image scan of a table)
- ★★★ make it available in a non-proprietary open format (e.g., CSV instead of Excel)
- ★★★★ use URIs to denote things, so that people can point at your stuff
- ★★★★★ link your data to other data to provide context

Le site http://5stardata.info/en/ propose pour chacune des 5 étapes de l’ouverture des données des exemples et explique les coûts et les bénéfices qui les accompagne. Les données utilisées pour les exemples sont issues de ‘*the temperature forecast for Galway, Ireland for the next 3 days*’.

---

## Qu’est-ce que le Web sémantique ?

> The **Semantic Web** provides a common framework that allows **data** to be shared and reused across application, enterprise, and community boundaries. It is a collaborative effort led by W3C with participation from a large number of researchers and industrial partners. It is based on the Resource Description Framework ( [RDF](https://www.w3.org/RDF/)).
>
> <https://www.w3.org/2001/sw/>

[W3C Data Activity](http://www.w3.org/2013/data/)

#### Principes

- [Tim Berners-Lee, James Hendler et Ora Lassila. « The Semantic Web. » *Scientific American*, May 2001.](http://www.sciam.com/article.cfm?articleID=00048144-10D2-1C70-84A9809EC588EF21&catID=2)
- [Tim Berners-Lee. Linked Data. 2009 [2006\].](http://www.w3.org:80/DesignIssues/LinkedData.html)

???

Le Web sémantique fournit un cadre de travail commun qui permet le partage et le réemploi de données à travers les frontières applications, entrepreneuriales ou communautaires. C’est un effort effort collaboratif porté par le W3C avec la participation de nombreux chercheurs et partenaires industriels. Il est basé sur le cadre de description RDF.

> The **Semantic Web** provides a common framework that allows **data** to be shared and reused across application, enterprise, and community boundaries. It is a collaborative effort led by W3C with participation from a large number of researchers and industrial partners. It is based on the Resource Description Framework ( [RDF](https://www.w3.org/RDF/)). See also the separate [FAQ](https://www.w3.org/2001/sw/SW-FAQ) for further information. 
>
> <https://www.w3.org/2001/sw/>

Le Web sémantique est un web de données. Il concerne le partage de format, l’intégration et la combinaison de données issues de sources diverses. C’est aussi un ensemble de standards et de langages destinés à documenter la manière dont les données sont en rapport avec les objets du monde réel. C’est une infrastructure technique qui permet à des personnes ou des machines d’accéder à des données connectées entre elles.

---

## Web de document .red[vs] Web de données

![img](/Users/emmanuelchateau/Documents/enseignements/msl6517/md/imagesMSL/webDeDonnees.png)

???

- Qu’est-ce que le web sémantique

  ### Le projet initial du web

  Le rêve du web était de créer une plateforme de collaboration et de communication collaborative qui permette de partager de l’information en établissant un espace informationnel universel pour l’information et les services.

  cf. **A proposal**, un web CRUD (CREATE, READ, UPDATE, DELETE) !

  Partage de documents par l’intermédiaire de l’hypertexte

  ### Web de documents vs Web de données

  Là où le web classique avait été développé comme un web de documents, le web sémantique est un web de données.

  - un web sur lequel ce ne sont plus les documents qui sont liés par des hyper liens mais l’information elle même qui est publiée et partagée de manière distribuée sur le réseau.

  cf. [Tim Berners-Lee: The next Web of open, linked data](https://youtu.be/OM6XIICm_qo) 2009

---

Le web sémantique et le web de données ouvertes et liées

Une manière d’utiliser le web

Ressources > identifiants > représentation

## Resources, Représentations et Identifiants

- Toute information pouvant être nommée peut être une **ressource**
- Une ressource peut recevoir plusieurs **représentations**
- Les ressources peuvent être **identifiées** sur le web.

Axioms of Web Architecture: 3, https://www.w3.org/DesignIssues/Generic

A Short History of "Resource" in web architecture. https://www.w3.org/DesignIssues/TermResource.html

---

background-image: url(imagesMSL/rdf.jpg)

.footnote[Diapositives Fabien Gandon INRIA]

???

Une grammaire de description universelle

¶ Resource

une page, une image, une vidéo, un concept,

n’importe quoi...

¶ Description caractéristiqeus et relation entre les ressources

¶ Format un modèle de données et des syntaxes pour la description

Recommandation W3C depuis 2004, version 1.1 en 2014

<https://www.w3.org/standards/techs/rdf#w3c_all>

#### RDF

Structurer les descriptions en informations atomiques sous la forme : sujet verbe prédicat. **RDF est avant tout un modèle de données basées sur des arcs.**

RDF a été inventé au cours des années 2000 dans l’idée de pouvoir disposer d’un modèle d’organisation des données. 

RDF signifie Resource Description Format. Resource ici est entendu de manière très très large, il peut s’agir d’un fichier, d’une image, d’une personne, d’un concept qui sont toutes des resources. L’idée sera de donner des identifiants à ces ressources afin de pouvoir les combiner sur le web.

cf. <https://www.w3.org/TR/rdf11-primer/>

### Motivations pour la création du format

- L’idée générale de RDF n’est pas de remplacer XML qui code avant tout les données, mais pour **coder des métadonnées**, il s’agira d’associer des informations à la page web. Le format est donc d’abord destiné à faire du web métadata.
- On voulait également pouvoir **disposer d’un modèle ouvert**. Le format est entièrement connu et standardisé et pas sous forme binaire.
- L’idée était aussi de pouvoir avoir des **métadonnées traitables en dehors de leur environnement de création**.
- Il s’agissait aussi d’être capable de **combiner l’information entre les applications**
- Traitable par la machine

### Buts de la conception

- On souhaitait pouvoir disposer d’un **modèle ouvert super simple de données**.
- On souhaitait également pouvoir disposer d’une **sémantique formelle qui permet des inférences**
- Disposer d’une sérialisation XML (même si on dispose aujourd’hui d’autres types de sérialisations) en intégrant les types XML
- Permettre à tous de créer des faits (des contenus)

---

background-image: url(imagesMSL/rdf01.png)

---

background-image: url(imagesMSL/rdf02.png)

---

background-image: url(imagesMSL/rdf03.png)

---

background-image: url(imagesMSL/rdf04.png)

---

background-image: url(imagesMSL/rdf05.png)

---

background-image: url(imagesMSL/rdf06.png)

---

background-image: url(imagesMSL/rdf07.png)

---

background-image: url(imagesMSL/rdf09.png)

???

### Rappel : des URI pour identifier ce qui existe

- URL identifier ce qui existe sur le web
- URI identifier sur le web, ce qui existe
- IRI identifier ce qui existe

### Des formats de représentation

- Resource
- Format

Les ressources (sujet, objet) et leurs relations (prédicat) sont identifiées par des IRI afin de les reconnaître et de pouvoir les manipuler par des machines.

L’objet du triplet peut être une ressource représentée par un IRI ou un littéral (une simple chaîne de caractères).

L’astuce est que le sujet est ce qu’on appelle un URI. L’idée est ici de disposer d’un indicateur unique à travers le monde. Celui-ci prend souvent la forme d’une URL. Certains organismes pouvant s’organiser pour créer des URIs, par exemple Wikipédia.

Le sujet est un URI, l’objet est un URI, et le prédicat est un URI. Tout cela peut donc être nommé. L’objet peut toutefois aussi être une constante (un nombre, une chaîne, etc.).

---

## Resource Description Framework .red[RDF]

![img](/Users/emmanuelchateau/Documents/enseignements/msl6517/md/imagesMSL/example-graph.jpg)

<https://www.w3.org/TR/rdf11-primer/>

???

## Assertions simples

sujet —> prédicat —> objet

Le principe de RDF est d’exprimer l’information sous forme de propositions simples qui prennent la forme "sujet, verbe, complément", ou "sujet, prédicat, objet".

Ces phrases sont appelées "triplets" 

L’idée est de construire un graphe dans lequel on aura des neuds. Dans un graphe RDF on a deux nœuds et un arc orienté. Dans une déclaration RDF on a un sujet, un objet et un prédicat.

C’est la base du système.

Sujet —> Prédicat —> Objet

Le **sujet** est toujours un IRI. Toute **ressource** sur laquelle on veut formuler une assertion (sujet) doit disposer d’un IRI. Les ressources sont typées par une **classe**.

Le **prédicat** est toujours un IRI. Il permet d’exprimer les **propriétés** des ressources ou la nature des relations des ressources entre elles.

L’**objet** peut être un IRI ou un littéral (une simple chaîne de caractères)

Les **classes** et les **propriétés** sont déclarées dans des vocabulaires ou des ontologies pour faciliter leur réutilisation.

---

background-image: url(imagesMSL/example-multiple-graphs.jpg)

???

Sujet —> Prédicat —> Objet

Le **sujet** est toujours un IRI. Toute **ressource** sur laquelle on veut formuler une assertion (sujet) doit disposer d’un IRI. Les ressources sont typées par une **classe**.

Le **prédicat** est toujours un IRI. Il permet d’exprimer les **propriétés** des ressources ou la nature des relations des ressources entre elles.

L’**objet** peut être un IRI ou un littéral (une simple chaîne de caractères)

Les **classes** et les **propriétés** sont déclarées dans des vocabulaires ou des ontologies pour faciliter leur réutilisation.

---

background-image: url(imagesMSL/example-multiple-graphs-iris.jpg)

---

## La pile des technologies du web sémantique

![img](/Users/emmanuelchateau/Documents/enseignements/msl6517/md/imagesMSL/sw_layercake.png)

???

### Fondements technologiques du LOD

- Un **système d’identification fiable** et pérenne pour identifier les ressources (URI, IRI)
- Une **grammaire pour la description et des syntaxes** (RDF, RDF/XML, N3, Turtle, JSON-LD, etc.)
- des **ontologies** exprimées sous une forme compréhensible par les machines (SKOS, RDFs, OWL)
- un **protocole et un langage de requête** et de manipulation de données (SPARQL)

### La pile technologique du web sémantique

Voici une visualisation réunissant les différentes technologies du web sémantique et la manière dont elles s’articulent les unes avec les autres. Ce graphique est une version modifiée de la visualisation Semantic Web technology stack visualization créée par Benjamin Nowack.

- Plateforme du web
- syntaxe / structure de représentation de la connaissance
- requêtes
- modèles sémantiques (ontologies, vocabulaires) + rules

---

## .red[CIDOC-CRM] Objectifs

- #### Permettre .red[l’échange d’information et l’intégration de sources de données hétérogènes] dans le domaine de l’information sur le patrimoine culturel 

- #### .red[Fournir des définitions sémantiques] et des clarifications nécessaires pour transformer des sources de données disparates, localisées en une ressource globale cohérente, au sein d’une institution ou sur l’internet 

- #### Une .red[perspective est supra-institutionnelle et abstraite de tout contexte local]. Cet objectif détermine les constructions et le niveau de détail du CRM. 

### **Exprimé sous la forme d’une ontologie formelle** 

???

> Le modèle conceptuel de référence (CRM) CIDOC fournit des définitions et une structure formelle pour la description de concepts implicites et explicites et leurs relations qui s’utilisent dans la documentation du patrimoine culturel.
>
> http://www.cidoc-crm.org/ 

- promouvoir compréhension partagée de l’information culturelle
- cadre de travail sémantique commun extensible
- liant sémantique pour médier des sources d’information hétérogènes

---

## .red[CIDOC-CRM] Historique

- .red[mars 1996], modélisation orientée objet 
- .red[1999], première version du CIDOC, processus de normalisation 
- .red[2005], DTD XML CRM-Core
- .red[2006], norme [ISO 21127:2006](http://www.iso.org/iso/catalogue_detail?csnumber=34424)
- .red[c. 2006], harmonisation avec [FRBR ((Functional Requirements for Bibliographic Records / Fonctionnalités requises des notices bibliographiques)](http://www.bnf.fr/fr/professionnels/modelisation_ontologies/a.modele_FRBR.html)
- .red[2014], version 5.0.4 publiée sous [ISO 21127:2014](http://www.iso.org/iso/catalogue_detail?csnumber=57832)

???

Un modèle conceptuel de référence

http://cidoc-crm.org

[ISO 21127](http://www.iso.org/iso/iso_catalogue/catalogue_tc/catalogue_detail.htm?csnumber=34424)

- les catégories d’information du CIDOC
- le modèle relationnel
- un modèle orienté-objet (depuis 1995)

Exprimer la sémantique sous-jascente des bases de données

## Définition

- **Exprime la sémantique sous-jascente des structures de la documentation sur le patrimoine muséographique**
- une formalisation des connaissances = concepts et relations portant sur les états de choses possibles dans un domaine
- une explication partagée plutôt qu’une structure commune de données (non prescriptif : ne dit pas ce qu’il faut décrire ni comment, mais permet d’interpréter les descriptions effectivement produites par les musées)
- accessible aux humains (documentation textuelle) et aux machines (OWL, etc.) pour permettre l’échange et l’intégration de données, la recherche fédérée, etc.

## Utilisation

- Aide intellectuelle pour l’élaboration de schémas de méta-données, de formats, de profils 
- Analyse de sources de données existentes à des fins d’intégration de données ou de médiation entre sources hétérogènes : « identifier les éléments qui ont une sémantique commune » 
- Format de transfert à des fins de migration ou d’intégration de données
- Ontologie informatique en vue d’une publication sous forme de données liées 

---

Un modèle orienté-événement

@todo

---

## Erlangen CRM / OWL

http://erlangen-crm.org

@todo

???

## Les ontologies

en sciences de l’informatique, une ontologie est une spécification formelle d'un modèle conceptuel lisible par la machine dans laquelle les concepts, propriétés,relations, fonctions, contraintes et axiomes sont explicitement définis

une description formelle explicite des concepts partagés dans un domaine donné et des relations entre ces concepts

- contient des définitions lisibles en machine des concepts (classes) et de leurs relations
- caractéristiques et attributs du concepts (rôles ou propriétés)
- restrictions sur les attributs (facettes ou restrictions de rôles)
- permet de formuler des raisonnements

une ontologie définit **une conceptualisation commune** pour une communauté qui a besoin de partager l’information dans un certain domaine

<https://www.w3.org/standards/techs/owl#w3c_all>

- un langage déclaratif pour exprimer des ontologies.
- plus riche que RDFs

Modélisation de base : 

- classes et instances
- hiérarchies de classes
- propriétés d’objets
- hiérarchies de propriétés
- Restrictions sur les propriétés
- égalité des individus
- types des valeurs de propriétés

---

Formats d’échange LIDO

@todo

---

Complexité du modèle

exemples

@todo

---

Swiss Art Research Infrastructure (SARI)

https://www.sari.uzh.ch/en.html

Université de Zurich

@todo

---

Patrons JSONLD

@todo

???

JSON-LD is a lightweight Linked Data format. It is easy for humans to read and write. It is based on the already successful JSON format and provides a way to help JSON data interoperate at Web-scale. JSON-LD is an ideal data format for programming environments, REST Web services, and unstructured databases such as CouchDB and MongoDB.

JSON-LD 1.1 https://w3c.github.io/json-ld-syntax/

---

Logiques de stock, et logiques de production

---

Limites du modèle CIDOC

@todo

exemples

- personnes
- performances
- expositions

---

DOnnées Patrimoniales HEritage DAta DOPHEDA

https://chin-rcip.github.io/collections-model/

tropy://project/current/items/311/312

@todo

