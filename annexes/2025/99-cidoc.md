## cidoc

Boeuf, Patrick Le. 2012. « De la sémantique des inventaires aux musées en dialogue : la modélisation CIDOC CRM ». https://hal-bnf.archives-ouvertes.fr/hal-00807664.

Distingue deux grandes catégories philosophiques

- Entités temporelles *E2_Temporal_Entity* (processus, endurants)
- Entités persistantes *E77_Persistent_Item* (perdurants, substances)

Une entité temporelle est quelque chose qui se passe dans le temps et dans l’espace, un état ou un changement d’état (un événement)

Le rôle des entités temporelles consiste essentiellement à mettre en relation ce qui est décrit dans les inventaires (objets matériels, créations de l’esprit, artistes, etc.) avec des lieux *E53_Place* et des intervalles de temps *E52_Time-Span*

E4_Period, ensemble cohérent de phénomènes ou de manifestations culturelles limités dans l’espace et le temps. Se subsume en l’événement E5_Event qui détermine la caractérisation d’une entité temporelle comme événement : c’est le fait qu’elle entraîne un changement d’état dans le monde matériel.

Trois types spécifiques d’événement sont explicités dans le modèle

- début d’existence *E63_Beginning_of_Existence*
- fin d’existence *E64_End_of_Existence*
- activité *E7_Activity*

La notion d’activité implique l’intentionnalité d’un agent humain. Mentionnant par exemple la création *E65_Creation*, c’est à dire l’activité par laquelle on donne naissance à un nouvel objet conceptuel *E28_Conceptual_Object* et à la production *E12_Production* qui débouche sur l’existence d’une nouvelle chose matérielle fabriquée E24_Physical_Man-Made_Thing.

Création et production sont donc deux cas particuliers ayant un caractère d’intentionnalité, de début d’existence.

Notion de Modification *E11_Modification*, opposée à la transformation *E81_Transformation* qui fait perdre à l’objet son identité pour donner naissance à un nouvel objet.

« Affectation d’attribut » (*E13 Attribute Assignment)* qui permet de contextualiser le discours tenu sur un objet.

### Les entités persistantes

Les entités persistantes définies par le CIDOC CRM se répartissent en deux grandes catégories

- Acteur *E39_Actor*, personnes physiques, collectivités, groupes informels
- Chose *E70_Thing*, chose matérielle *E18_Physical_Thing* et objet conceptuel *E28_Conceptual_Object*

La classe objet conceptuel recouvre les créations de l’esprit. On y trouve notamment des notions telles que celles d’image *E38_Image* et d’objet linguistique *E33_Linguistic_Object* mais aussi d’appellation *E41_appellation* et de type *E55_Type*

Propriété P131 qui relie un acteur et une appellation d’acteur E82_Actor_Appelation

> E39 Acteur *P131 est identifié par (identifie)* E82 Appellation d’acteur {instance = « Michel-Ange »}

Exemple

Titre : Le Radeau de la Méduse

Auteur/exécutant : Géricault Théodore 

Millésime création/exécution : 1818-1819

> E22 Objet fabriqué P65 présente l’item visuel E38 Image
>
> ​	E38 Image P102 a pour titre E35 Titre {instance = « Le Radeau de la Méduse »}
>
> E22 Objet fabriqué P108B a été produit par E12 Production
>
> ​	E12 Production P14 réalisée par E21 Personne
>
> ​		E21 Personne P131 est identifié par E82 Appellation d’acteur {instance = « Géricault Théodore »}
>
> E12 Production P4 a pour durée E52 Durée
>
> ​	E52 Durée P78 est identifiée par E50 Date {instance = « 1818-1819 »}

> La sémantique contenue sous une forme concise et synthétique dans la notice de la base Joconde est donc « dépliée », explicitée dans le formalisme du modèle CIDOC CRM. Le principe est de permettre à deux bases de données conçues dans des formats différents de pouvoir dialoguer entre elles à travers leurs traductions respectives vers la même explicitation opérée par le CIDOC CRM: quelle que soit la structure d’une base de données muséographique, elle devrait normalement toujours exprimer l’idée qu’une personne dénommée « Géricault Théodore » a joué un rôle actif dans la production d’un objet matériel support d’une image intitulée « Le Radeau de la Méduse », et que cette production s’est déroulée sur un laps de temps identifié par la tranche de dates « 1818-1819 ».

E84_Information_Carrier P108B_was_produced_by E12_Production

​	E12_Production P4_has_time-span E62_Time-span

​	E12_Production P14_carried_out_by E21_Person

### E65 Creation

http://www.cidoc-crm.org/Entity/e65-creation/version-6.2.1

[P94 has created (was created by)](http://www.cidoc-crm.org/Property/p94-has-created/version-6.2.1) [: E28 Conceptual Object](http://www.cidoc-crm.org/entity/e28-conceptual-object/version-6.2.1)

### E73 Information Object 

http://www.cidoc-crm.org/Entity/e73-information-object/version-6.2.1

E36 Visual Item

http://www.cidoc-crm.org/Entity/e36-visual-item/version-6.2.1



E21_Person P2_has_Type E55_Type P1_is_identified_by E41_Appelation

E45_Creation P14