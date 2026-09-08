## Conception de bases de données (modèle Entités-Assocations)

https://web.maths.unsw.edu.au/~lafaye/CCM/merise/concintro.htm

**La modélisation consiste à passer du monde réel à sa représentation informatique. La mise au point d’un système d’information se déploie souvent en plusieurs étapes pour parvenir à son intégration dans un SGBD-R et permettre la manipulation des données par le langage SQL.**

Classiquement, le processus de modélisation des données passe par deux phases :

- Réalisation d’un modèle conceptuel
- Traduction en un modèle relationnel

> Le premier niveau de modélisation, dit conceptuel, consiste en une phase d’analyse du problème réel. Cette phase est assez délicate et permet de définir les données à utiliser, leur mode d’évolution dans le temps et les relations entre elles. C’est le moment où l’on se pose les questions essentielles comme celle de savoir à quel usage on destine le modèle informatique que l’on est entrain de constituer.
>
> Ce travail est réalisé par des spécialistes de l’analyse. Il s’exprime dans un formalisme de type entité-association. Il existe d’autres types de formalismes comme le formalisme UML ou Merise (cf. ANNEXE).
>
> Le second niveau de modélisation, dit relationnel, conduit à élaborer l’ensemble des objets manipulables par un SGBD-R. Ce travail est souvent réalisé par l’architecte de données, ou un administrateur de SGBD. Il peut être découpé en deux étapes :
>
> - la conception de modèle logique (représentation en tables indépendantes du SGBD)
> - la traduction en un modèle physique (propre à un SGBD spécifique). Tous les SGBD n’ont pas les mêmes caractéristiques du langage SQL.

La modélisation d’un domaine pour la création d’un système de gestion de base de données est une opération difficile. On passe donc souvent par des modélisations intermédiaires afin de faciliter ce travail. Le modèle entités-associations est une modélisation relativement simple et naturelle pour représenter le monde réel à partir des concepts d’entité et d’association. Ce modèle basé sur la théorie des ensembles et des relations se prétend universel et est indépendant de toute implémentation logicielle.

Ce modèle s’inscrit dans le cadre de la méthode de modélisation Merise (Méthode d’Étude et de Réalisation Informatique pour les Systèmes d’Entreprise) qui est particulièrement répandue en France dans la communauté informatique des systèmes d’information et des bases de données. La méthode Merise est une méthode d’analyse, de conception et de réalisation de systèmes d’information. Elle permet de valider des choix de conception et de guider l’implémentation, par son formalisme, c’est aussi un outil de communication sur le système. D’autres méthodes standardisées sont également utilisées dans ce domaine comme UML.

La méthode Merise distinguer plusieurs niveaux de modélisation :

- le **niveau conceptuel** où le *modèle conceptuel des données* MCD décrit les entités du monde réel en termes d’objets, de propriétés et de relations indépendamment de toute technique d’organisation et d’implémentation. Ce modèle se concrétise le plus souvent dans la production d’un diagramme entités-associations qui représente la structure du système d’information du point de vue des données.
- le **niveau logique** : le *modèle logique des données* (MLD) précise le modèle conceptuel par des choix organisationnels. Choix d’une implémentation technique.
- niveau physique : où le *modèle physique des données* (MPD) permet d’établir de manière concrète la manière dont le système sera mis en place.

## Le modèle conceptuel de données (MCD)

Un schéma conceptuel représente :

- Les faits et les évènements qui décrivent le monde à modéliser. 
  Exemple : une compagnie aérienne, ses avions et ses pilotes.
- Certaines contraintes. 
  Exemple : un pilote ne doit vole que s’il détient une licence en cours de validité et une qualification correspondant au type d’avion.
- Les différentes techniques de MCD :
  - Entité-Association (en anglais E-R pour Entity Relationship)
  - Modèle binaire
  - Modèle Z

Un MCD prend généralement la forme d’un diagramme qui représente des entités et des associations. Pour réaliser un tel diagramme, dans le monde professionnel, les spécialistes s’aident d’outils logiciels graphiques et de différents formalismes. Ces outils sont parfois capables de générer le modèle logique (le plus souvent le modèle relationnel) de la base. On se sert ensuite d’un script (le plus souvent en SQL) pour implémenter les différentes tables et les contraintes dans le système informatique.

Le problème le plus couramment rencontré au sein des bases de données mal conçues est la redondance. Cette faute entraîne, à terme, des incohérences en modification, insertion et suppression de données, et rend la base peu performante.

## 2. Le modèle Entité-Association

**La production d’un modèle entité-association consiste à représenter, par un schéma standardisé, les différents éléments constitutifs du système d’information, appelés attributs (exemple : nom, âge, ...), et les relations qui les unissent, appelées associations.**

Une manière simple de modéliser est de décrire la réalité par une phrase : **Le sujet et le complément représentent des entités, et le verbe l’association.**
Exemple : un utilisateur (entité) poste (association) une news (entité).

La représentation du modèle entités-associations s’appuie sur trois concepts de base :

- l’objet ou entité,
- l’association, 
- la propriété.

2.1. Entité

Définition : Une entité est un objet, une chose concrète ou abstraite qui peut être reconnue distinctement et qui est caractérisée par son unicité.

Il faut noter que les entités ne sont pas représentées sur un modèle entité-association.

Définition: Un type-entité désigne un ensemble de d’entités qui possèdent une sémantique et propriétés communes.

Une entité est une occurrence ou instance de son type-entité. Par abus de langage, le terme entité est régulièrement utilisé pour désigner le type-entité et ses entités. Il ne faut cependant pas confondre ces deux notions.

2.2. Association

Comme pour l’entité, le terme d’association est utilisé pour désigner un type-association. Définition : Une association (ou relation) est un lien entre plusieurs entités.

2.3. Attribut et valeur
 Définition : Un attribut (ou propriété) est une caractéristique associée à un type-entité

ou à un type association.

2.5. Cardinalités d’un type-association

Définition : Les cardinalités d’une patte reliant un type-association et un type- entité précisent le nombre de fois minimal et maximal d’interventions d’une entité du type-entité dans une association de type-association. La cardinalité minimale doit être inférieure ou égale à la maximale.

https://laurent-audibert.developpez.com/Cours-BD/?page=conception-des-bases-de-donnees-modele-a

http://www.info.univ-angers.fr/~gh/Pluripass/Db/seance2-ModeleEA.pdf

https://app.diagrams.net/