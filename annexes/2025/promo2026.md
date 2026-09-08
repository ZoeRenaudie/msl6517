Bienvenue sur Framapad !

Framapad est un des nombreux projets de Framasoft, association d éducation populaire aux enjeux du numérique et des communs culturels.

➡ Comment commencer ?
• Renseignez votre nom ou pseudo, en cliquant sur l’icône « utilisateurs » en haut à droite.
• Choisissez votre couleur d’écriture au même endroit.
• Lancez-vous : écrivez sur votre pad !
• Les contributions de chacun⋅e se synchronisent « en temps réel » sous leur propre couleur.

➡ Comment sauvegarder ?
• Il n’y a rien à faire : le texte est automatiquement sauvegardé, à chaque caractère tapé.

----------------------------------------------------------------------------------------------------------------------------

# MSL6517 Introduction aux métadonnées culturelles

Pensez à lire les textes, ils devraient vous aider à faire les exercices !  

Donnez moi accès à vos documents svp ! Et mettez votre nom dans le nom du doc please
Google Drive : zoe.renaudie@gmail.com
Onedrive : zoe.renaudie@umontreal.ca

--------------------------------------------------------------------------------------------------------------------------------------

# 1er décembre - Linked Art

Anne-Julie: https://docs.google.com/document/d/1lvjVt_jMU-kWwOPrQz7MOHgxjFKmp63c3OcV1T7VFP0/edit?usp=sharing

Sophie : https://drive.google.com/file/d/1h_qaD6Nyrez8jDTyuGx__S59h2dY8gyo/view?usp=sharing

Hugo: https://drive.google.com/file/d/1AnxxMxMKt3trTi7hFcIeKFBO07jnTPu-/view?usp=sharing
https://app.diagrams.net/#G1AnxxMxMKt3trTi7hFcIeKFBO07jnTPu-#%7B%22pageId%22%3A%22IcZpeexxcDE9uRctHstA%22%7D

Suzanne
https://drive.google.com/file/d/1DKVvnCt-pvdfxMTWkrNZtbgt-mRYsVI0/view?usp=sharing

Ema : https://docs.google.com/document/d/1qDPWAiSH2ExpaUdFiN2GpG8spahx2n48kPOp1YZD_4A/edit?usp=sharing

Sandrine : 
https://drive.google.com/file/d/1QCY2ddmwOzhW3ZDayw27OKyGyZhYrzCH/view?usp=sharing 

Jade : https://drive.google.com/file/d/1if91rXwvdKIZUtaddnSrQVfPsdiqBUUZ/view?usp=drive_link

Simon : https://drive.google.com/file/d/1u4iaUb9C6tHS_wVQl9t6YuhNneHO5llc/view?usp=sharing

Jeanne:https://docs.google.com/document/d/14MggdO6O5CCMhm4EnDNOypOPofWRCLdArhmOsjGVkzI/edit?usp=sharing

Camila: https://udemontreal-my.sharepoint.com/:w:/r/personal/camila_maghraoui_hassani_umontreal_ca/_layouts/15/Doc.aspx?sourcedoc=%7B05325D00-0E19-45EC-92E2-36D4A9F503F8%7D&file=Document%202.docx&action=editNew&mobileredirect=true&wdOrigin=OFFICECOM-WEB.APPGALLERY%2CAPPHOME-WEB.BANNER.NEWBLANK&wdPreviousSession=cca6940d-7319-4dc4-9d32-7971a210b0f0&wdPreviousSessionSrc=AppHomeWeb&ct=1764544410103

# 24 novembre: Travail Open Refine

Suzanne
http://127.0.0.1:34333/#open-project
J'espère que le lien fonctionnera correctement.

Anne-Julie:
http://127.0.0.1:3333/project?project=2499918914274
Suggestions d'amélioration:
- Diviser les lieux de production (ville, province, pays)
- Diviser et préciser les dimensions (longueur, largeur, profondeur)
- Interopérabilité des autres musées avec qui le MAC a effectué des prêts

Hugo: http://127.0.0.1:3333/project?project=1831598312166
La réconciliation a moyennement fonctionnait et J'ai du l'a finir un par un en séparant les erreurs et les succès et travaillant sur les inconnues ou plusieurs match étaient possibles avec wikidata. Des 1880 j'ai pu avoir la réconciliation de 280 pour le reste de l'exercice

Les noms :
La base de données utilisait deux colonnes (nom, prénom), donc il a fallu faire une colonne qui rassemble les deux pour que ça match avec les noms complet de wikidata. Les noms d'artistes étaient parfois incomplets ou ambiguë (ex: Alog sans prénom). Aussi les groupes d’artistes dans les données a provoqué l'échec de la réconciliation pour ces lignes, car il ne pouvait pas les identifier comme une seule personne et des fois les groupes d’artiste se référer juste à l’entité et non les personnes qui la compose
Solution : normalisation des noms et des prénoms, dans le cas de groupe les artistes individuelles devraient être rejoutés dans des colonnes individuelle 
Les dates :
Les dates de wikidata incluent les mois et le jour, une information qui pourrait être utile pour le MAC  


Sophie :  mon ordinateur a beaucoup de difficulté à gérer la quantité de données, j'ai fait une version du fichier avec moi de données, mais même après l'avoir laissé charger les réconciliations Wikidata toute une nuit, ce n'est pas terminé malheureusement.

Voici une version avec moins de données - https://docs.google.com/spreadsheets/d/12aYFicJMtghlFwHgSnOk6AkTiUOVMKIy/edit?usp=sharing&ouid=103974704129631402859&rtpof=true&sd=true

Au cas où, voici ce que j'ai fait - Décomposer les champs lieu_naissance et lieu_mort en plusieurs champs ville_naissance, province_naissance, pays_naissance, ainsi que ville_mort, province_mort et pays_mort : fait en trois temps, séparateurs virgule, ferme la parenthèse et ferme la parenthèse une deuxième fois (pour se débarrasser de la parenthèse après la province ou l’État).
 
Réconcilier les noms des artistes à ceux de Wikidata : créer une colonne nom_complet (entre autres régler le problème du premier essai avec les multiples Adams et matcher avec Wikidata), puis réconcilier avec type Q483501 de Wikidata (artiste) / Q5 (être humain).
 
Enrichir la base de données du MAC en ajoutant l'identifiant Wikidata des artistes : utiliser « Add column with URLs of matched entities » en sélectionnant la colonne qui a été réconcilié avec le type Q483501 (artiste).
 
Enrichir la base de données du MAC en ajoutant les dates de naissance et de mort selon Wikidata : utiliser « Ajouter des colonnes à partir des valeurs réconciliées » - date_de_naissance et date_de_mort – les années sont déjà recensé dans la base de données – malheureusement, les données ne sont pas recensées ni disponibles (ou j’ai fait la mauvaise manipulation, parce que rien ne s’affiche).
 
La plus grande différence que je constate concernant les différents jeux de données est l’enjeux de noms et de lieux, qui, selon la langue et le jeu de données, ont une orthographe différente, ce qui peut compliquer les recherches.

Suggestions pour les améliorations :

- Ajouter les informations de base manquantes – le prénom (dans certains cas), les dates de naissance et de décès, ou le médium principal, par exemple.
 
- Effort de standardisation : nettoyer les données existantes, en les alignant avec Wikidata, ce qui permettrait aussi de récupérer certaines données manquantes.
 
- Subdivision de certaines colonnes / types de données, comme pour les dates de naissances et de décès, par exemple.

- Association de certaines colonnes - par exemple, une colonne avec le nom complet, pour faciliter la réconciliation et la recherche.
 
- Concernant les données bibliographiques de l’artiste : utiliser des systèmes et des autorités externes comme GETTY ou LCNAF pour le vocabulaire.


Ema : 
https://drive.google.com/drive/folders/1EMLJQtTuA5lIKRxYtcvGzplo5bPkteZb?usp=share_link

Sandrine : 
http://127.0.0.1:3333/project?project=2139299693420

Jade : http://127.0.0.1:3333/project?project=2108238861833
Beaucoup de difficultés avec l'accès. Souvent, mon ordinateur affichait des messages d'erreur ou n'arrivait pas à charger la page. J’ai tout de même tenté de faire le maximum.

    J’ai réussi à décomposer les champs demandés (mais encore là, j'arrive pas à enlever la parenthèse qui reste)

    La réconciliation pour le nom a été très longue (je ne sais pas si cela a bien fonctionné)

    Après plusieurs essais, je ne suis pas parvenue à ajouter les identifiants des artistes, ni à enrichir avec d’autres données... 

Amélioration : mieux subdiviser les colonnes (décortiquer les données), normaliser et standariser les termes

Camila: http://127.0.0.1:3333/project?project=1950445755048
Il était difficile de faire la réconciliation, l'opération a fait planter mon ordinateur plusieurs fois. (retenté avant le cours et ça a marché, manque ceux qui sont à reconcilier manuellement, je ne suis pas non plus arrivée à enrichir la base de données avec les identifiants, dates de naissances et morts selon wikidata) 
Améliorations:
    -meilleure normalisation des données serait idéale incluant comment elles sont notées ex. provinces entre paranthèses, noms de villes et régions multiples, ce qui rend la séparation des données difficile.
    -  Certaines informations semblent manquantes? (ex. nom complet des artistes ou stage name?)

Jeanne: http://127.0.0.1:3333/project?project=2551198116624
utilisation de formules (edit cell -> transform : formules :
value.replace(/^.*\((.*)\).*$/, "$1") 

value.replace(/\([^)]*\)/, "").trim()


Simon: https://drive.google.com/drive/folders/1GFlm1UrdHrjVv5ZCd9uCuwgMu5cGoWjk?usp=sharing

# 17 novembre:  Travail de groupe sur la mise en commun de données

Sophie Fox-Mauffette - Te Papa Tongarewa et Musée canadien de l'histoire

Champs de description communs :
    
Voici les champs de description communs entre les jeux de données du Te Papa Tongarewa et du Musée canadien de l’histoire. Pour réaliser l’exercice, j’ai utilisé les versions anglaises des catalogues en ligne.
Champs à vocabulaire et fonctions identiques : Materials, qui se nomme Materials dans les deux catalogues. Te Papa Tongarewa met aussi de l’avant les champs Materials Summary et Made of, qui remplissent des fonctions similaires.

Les champs de description suivants, bien que le vocabulaire soit différent, peuvent aussi être jugés équivalents considérant l’usage qu’en fait chaque catalogue. Le premier terme désigne l’appellation privilégiée par Te Papa Tongarewa, qui est séparée par un trait d’union de celle utilisée par le Musée canadien de l’histoire.

    Registration Number – Artifact Number

    Name – * titre au haut de la page web * 

    Classification et/ou Type of – Category

    Production et/ou Made by – Artist / Maker / Manufacturer

    Production – Date Made / Earliest / Latest (qui sont des composantes de l’onglet production de Te Papa Tongarewa).

    Place et/ou Made in et/ou Associated Places – Place Of Origin

    People & Organisations – Affiliation

    Dimensions – Measurements

    Explore more information – Searching for more ? (Rôle identique pour l’expérience de l’utilisateur)

 
Pour finir, voici les champs propres à chacun des catalogues, n’ayant aucun équivalent :

Te Papa Tongarewa

    Collection

    Credit line

    Technique et/ou Technique Used

    Overview

    Intended for

    Influenced by

    Belonged to

    Related records

    Publication (ou au pluriel)

    Topic (ou au pluriel)

 
Musée canadien de l’histoire

    Accession Number

    Geo-Cultural Code

    Department

    Cataloguing Status

    Rights and Permissions

 
Enjeux :

    En termes d’enjeux, j’en ai identifié quatre principaux. Le premier est la variabilité du vocabulaire utilisé pour décrire essentiellement les mêmes attributs, ce qui pourrait provoquer des ambiguïtés au moment d’une mise en commun. Par exemple, les termes Registration Number et Artefact Number désignent un attribut qui joue exactement le même rôle au sein des efforts de gestion de collection, ce qui n’est pas évident du fait des mots utilisés.

    Le deuxième est une différence quant aux détails qu’englobent certains champs : certains sont très précis, alors que d’autres pourraient être séparés en plusieurs sous-champs, ce qui complexifie les équivalences. Par exemple, le champ Production dans le catalogue de Te Papa Tongarewa regroupe à la fois la date de production, le lieu de production et le producteur (artiste ou artisan) de l'artefact, alors que le Musée canadien de l’histoire subdivise plutôt ces informations. Donc si l’on voulait trouver un équivalent au champ Production pour effectuer un partage d’information, il faudrait s’assurer d’inclure Artists / Maker / Manufacturer, Date Made, Earliest et Latest dans la liste des champs à transposer.

    Le troisième est la présence de champs très riches tels que Overview (Te Papa Tongarewa), qui n'ont parfois aucun équivalent au sein de l’autre catalogue, résultant en une perte d’information à moins d’intervenir, évidemment.

    Le dernier, mais non le moindre, est la présence de champs qui sont très spécifiques à l’institution propriétaire (ayant sans doute des fonctions gestionnaires / internes) tels que Department ou Geo-Cultural Code, qui se traduisent difficilement une fois sortis du contexte précis dont ils proviennent.


J’ai tenté d’identifier une ou quelques solutions par défis de mise en commun recensés ci-haut.
 
Pour l’enjeu de vocabulaire, il s’agirait de :
 

    Créer un glossaire commun pour fixer et officialiser les équivalences si le vocabulaire est différent.

    Tenter d’adopter certains systèmes tels que Dublin Core qui travaillent à harmoniser les termes utilisés.

 
Concernant le défi du détail, il faudrait :
 

    Décortiquer les champs complexes en sous-champs standardisés qui restent sous le même champ (pour éviter les pertes de précision tout en s’assurant de ne pas dénaturer les efforts de mappage du musée ou de l’institution culturelle.

 
Pour la question de l’absence d’équivalent des champs plutôt riches, je suggère :
 

    D’identifier clairement la présence (et la différence entre les) d’équivalents exacts, d'équivalents potentiels et les absences d’équivalents pour pouvoir être transparent quant aux données qui sont explicitement faciles à transposer, et celles qui posent problèmes.

    À la suite de cela, il serait important de documenter les cas sans équivalences pour qu'ensuite, à l’aide d’une méthodologie précise, mais propre à l’institution, on détermine sous quel champ il serait pertinent de loger  l'information pour éviter une perte de données.

 
Concernant la présence de champs spécifiques à l’institution :
 

    Comme pour le problème d’absence d’équivalence, il serait pertinent de loger les données pertinentes pour d’autres institutions au sein d’un dossier semblable à celui proposé par Spectrum lors de l’acceptation d’un don d’objet, par exemple, où toutes les informations répertoriées par l’institution ou l’individu précédent sont conservées. On y trouverait, par exemple, des champs comme Department. 


Ema et Anne-Julie:
https://docs.google.com/document/d/1mAR1LhjaykyIJ0_vcH8Kxnjut43G7XlJrlAfZnbLyz0/edit?usp=sharing

Hugo: https://docs.google.com/document/d/1zIhaHlFi4kXWrhl1i-roS4wg7YdL9CQTnGioIaDqRnw/edit?tab=t.0

#3 novembre : Sélection d’une solution informatique pour la gestion d’une collection

Suzanne Desormeaux
https://docs.google.com/spreadsheets/d/1xE2HmP-YAUpin3iqfuBKhwmpA7VQ6kl0ZmUeQ28QE4w/edit?usp=sharing

Anne-Julie Robitaille
https://docs.google.com/spreadsheets/d/1A0pHmVZpjewafO9Y93mRD8qV16dnIBNgrD_asZP7BcU/edit?usp=sharing

Sophie Fox-Mauffette -  https://udemontreal-my.sharepoint.com/:x:/r/personal/sophie_fox-mauffette_umontreal_ca/_layouts/15/Doc.aspx?sourcedoc=%7BA6A61F06-B315-41A8-9094-CDE44C41975A%7D&file=Comparaison%20-%20LOGICIELS%20DE%20GESTION.xlsx&action=default&mobileredirect=true

Camila: https://udemontreal-my.sharepoint.com/:x:/r/personal/camila_maghraoui_hassani_umontreal_ca/_layouts/15/doc2.aspx?sourcedoc=%7B71938260-2922-44B3-BA42-4E329F826F7F%7D&file=Book.xlsx&action=editNew&mobileredirect=true&wdOrigin=OFFICECOM-WEB.APPGALLERY%2CAPPHOME-WEB.BANNER.NEWBLANK&wdPreviousSession=52988004-7a34-4f6f-a345-cb7fd7973554&wdPreviousSessionSrc=AppHomeWeb&ct=1762126707897

Jade : https://docs.google.com/spreadsheets/d/1zglfhuRgtGwBxc9lD1O8mUpyRZvGqR2VeooTBgO27F8/edit?usp=sharing

Ema : 
https://docs.google.com/spreadsheets/d/15dieG5sIefl2qyhqu6eK1TyzoW_S6M-GxcB30-8j1v8/edit?usp=sharing
    
Jeanne : https://udemontreal-my.sharepoint.com/:x:/r/personal/jeanne_beaudonnet_umontreal_ca/_layouts/15/Doc.aspx?sourcedoc=%7BCDB919E3-F298-4629-BF91-054EED69B602%7D&file=liste-criteres-logiciels.xlsx&action=default&mobileredirect=true&wdOrigin=OUTLOOK-METAOS.FILEBROWSER    
Sandrine : 
https://docs.google.com/document/d/1TqNocEpvj-0rC4UIafcYKH8l9HA-ozsEHqXFopc83Ho/edit?usp=sharing

Simon : https://docs.google.com/spreadsheets/d/1IBbkrl579hMpry1RFzh9ND51_2cdB_tK/edit?usp=sharing&ouid=109396661764452632399&rtpof=true&sd=true

Hugo: (Peut au besoin montrer a quoi ressemble l'interface de Collectionspace et de la base de donnée) https://docs.google.com/spreadsheets/d/1K2JRSwsBx7AgpWgfPEfov-rP23vFB2CiVqxDwulimQM/edit?gid=0#gid=0

--------------------------------------------------------------------------------------------------------------------------------------

#27 octobre : Produire un diagramme entité-association des informations de catalogage sur un artefact

Ce schéma n'est pas un mapping de vos objets, il ne doit pas y avoir les données sur les objets de vos collections. Ça doit ressembler à ce qui est proposé dans ce cours : https://laurent-audibert.developpez.com/Cours-BD/?page=conception-des-bases-de-donnees-modele-a
Ou la page 12 de ce document, vous avez 3 différents types de manière de représenter votre schéma : https://gilles-hunault.leria-info.univ-angers.fr/Pluripass/Db/seance2-ModeleEA.pdf

Suzanne
https://viewer.diagrams.net/?tags=%7B%7D&lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&dark=auto#G1wh7hj-6GHHeFyT_tkgWZcO-bK9bfin50
https://drive.google.com/file/d/1wh7hj-6GHHeFyT_tkgWZcO-bK9bfin50/view?usp=drive_link

Ema : 
https://docs.google.com/presentation/d/1VZS8wnkgBf0HtVVYwiLRptZj5Ya0hBiC/edit?usp=sharing&ouid=115081308624442547122&rtpof=true&sd=true 
    
Anne-Julie:
https://drive.google.com/file/d/1nHs4PPkuTqOf73yOfiHcnRVtqCu48uVH/view?usp=sharing

Hugo:
    V1: https://app.diagrams.net/#G1XPN3giUtS5TSGz6Y2cwbS-UfiPRprd9o#%7B%22pageId%22%3A%22PzlH6zwW2vP7hJbPCEhX%22%7D

Jeanne : https://app.diagrams.net/#G1oKdvNyxEQXBihMa8xNiG__0AV4rb9n2q#%7B%22pageId%22%3A%22n67kdDY1PJUlu6jsWvUU%22%7D

Sophie Fox-Mauffette: https://drive.google.com/file/d/1vjetwsWd03nE3bXfTlEyEvTRk9xui1zW/view?usp=drive_link


Camila: https://drive.google.com/file/d/1ztwofuX74OxKEM6cyX7MCKVWFOSboG6R/view?usp=sharing

Sandrine : https://drive.google.com/file/d/1EPjbdbykNWsFkAFTfGkw1htOfs3CDfEN/view?usp=sharing

Jade : 
    Essaie 1 : https://drive.google.com/file/d/11XOz3Wc9IY1Dm5lWDaKcq4MFA9SLh-0p/view?usp=sharing
    Essaie 2 : https://drive.google.com/file/d/1yFOcAd3VVUkb-MHpjat4QGOC1uMKjmLJ/view?usp=sharing

Simon : https://udemontreal-my.sharepoint.com/my?id=%2Fpersonal%2Fsimon%5Fgravel%5F3%5Fumontreal%5Fca%2FDocuments%2FTP5%2ESimonG%2Edrawio%2Epng&parent=%2Fpersonal%2Fsimon%5Fgravel%5F3%5Fumontreal%5Fca%2FDocuments&ga=1

https://drive.google.com/file/d/1Tii91giZMFlRQoWtGrC652aT38vKHs0V/view?usp=sharing


--------------------------------------------------------------------------------------------------------------------------------------
#groupes 


-----

#6 octobre : Traiter sous forme tabulaire les informations de catalogage de 5 artefacts

Suzanne Desormeaux
McCord Stewart Museum (1).xlsx

Anne-Julie
https://docs.google.com/spreadsheets/d/10Is5NGYeJnP8LQKOKKhyquVwJZw5L9j3jHsmp_bXHmk/edit?usp=sharing

Ema Holgado
https://docs.google.com/spreadsheets/d/1Pa_uk1T3_jaNcWrsYxwViwk9N3mu7I4hVFNc0OMXg4Q/edit?usp=sharing

Sophie Fox-Mauffette
https://docs.google.com/spreadsheets/d/1mAsUZWcSkrcV-09sP1e5hqpiou-gZZN_BCOvSLjuF20/edit?usp=sharing

Jade
https://docs.google.com/spreadsheets/d/1mL5nWKoG3AZqzds82N4o4lS7vJ93gnLvL4AdO2jB-54/edit?usp=sharing

Camila: https://udemontreal-my.sharepoint.com/:x:/r/personal/camila_maghraoui_hassani_umontreal_ca/_layouts/15/Doc.aspx?sourcedoc=%7BF4ECB53C-49C8-4576-965B-14EC0C6C31D4%7D&file=Book.xlsx&action=editNew&mobileredirect=true&wdOrigin=WORDONLINE.SHELL%2CAPPHOME-WEB.BANNER.NEWBLANK&wdPreviousSession=6e3c28f3-f62f-44c7-b2e6-268b43d5243e&wdPreviousSessionSrc=AppHomeWeb&ct=1759366584106

Simon
https://udemontreal-my.sharepoint.com/:x:/g/personal/simon_gravel_3_umontreal_ca/EbyS0XJq-SFJo2B6b2pnnk0B9cro1eeHrmErckkdooimqA?e=YrXdZ0

Jeanne
https://udemontreal-my.sharepoint.com/:x:/r/personal/jeanne_beaudonnet_umontreal_ca/_layouts/15/Doc.aspx?sourcedoc=%7BAA0DAAA0-F9B1-46C8-AE1A-5D3E91DB1AB9%7D&file=catalogue%20artefacts%20MSL%2006.10.xlsx&action=default&mobileredirect=true&wdOrigin=OUTLOOK-METAOS.FILEBROWSER

Sandrine Dufour
https://docs.google.com/spreadsheets/d/1Vsq4m7PQI7Z4jJ4u3Q3F9_1HRuO7w3ovy7ZOwePPaq0/edit?usp=sharing

Hugo: https://docs.google.com/spreadsheets/d/1LEnjOHkfrynq4SszoTJFhF-fWAl8ZytySrhLPdPJMno/edit?usp=sharing


--------------------------------------------------------------------------------------------------------------------------------------

Hugo:
Identification :
Numéro d’objet: 71.1930.13.33
Nom de l’objet:  Récipient ornithomorphe
Courte description: Vase tripode en forme d'oiseau aux ailes déployées, queue et long cou. Sur le dos, ouverture ovale. Les ailes et la queue portent des rayures assez profondes. Bec cassé.
Emplacement actuel: Pas exposé
Propriétaire: musée du Quai Branly
Technique : Terre cuite rouge engobée
Dimensions : (Hauteur) 12,1 cm (Largeur) 10,2 cm (Longeur) 14,6 cm
299 grammes
 
Informations sur les associations :
Peuple Associes : Créole
Lieux associes : Amérique> Amérique du Sud> Chili> Araucanía> Temuco
Organisations associées : Gouvernement du Chili, Musée de l'Homme (Amérique)
 
Informations sur la production :
Date de production: début 20e siècle
Lieu de production: Temuco, Chili

Sophie Fox-Mauffette

Information sur l’identification de l’objet :
Numéro d’objet unique : ME017455
Nom de l’objet : "Hinewaitapu" Ceramic Sculpture (female)
Contenu – description : Cette sculpture d’argile beige représente une femme aux cheveux courts apposant sur son ventre ses deux mains. L’œuvre fait écho au caractère spirituel de la femme au sein de la tradition maorie, le préfixe du titre, « hine », signifiant fille, « wai », signifiant eau, et le suffixe, « tapu », référant en même temps au sacré et à l’interdit d’une personne, d’un objet, ou d’un lieu.
Contenu – type d’objet : sculpture, céramique
Dimensions : 540 mm x 950 mm x 280 mm
Matériaux : uku (argile)
 
Information sur l’historique et les associations à l’objet :
Peuples associés : Ngāti Kurauia, Ngāti Tūwharetoa, Te Āti Haunui a Pāpārangi, Ngāti Uenuku (Te Āti Awa)
Lieu associé : North Island, Nouvelle-Zélande
Collection associée : Collection Taonga Māori
 
Information de la production de l’objet :
Personne de production de l’objet : Paerau Corneal (1961 - )
Lieu de production de l’objet : Kekerengu, Kaikōura, Canterbury, Nouvelle-Zélande
Technique : sculpture, gravure
 
Notes sur la comparaison entre les métadonnées disponibles au sein du catalogue en ligne et celles que SPECTRUM suggère de recueillir :

Te Papa Tongarewa offre une multitude de métadonnées, et les bases de SPECTRUM sont effectivement respectées. Les titres, les numéros d’inventaire, le statut de l’objet, et la provenance sont facilement identifiables, et les données techniques telles que les dimensions, les matériaux, et toutes informations concernant la production ou la collecte sur le terrain sont généralement disponibles. Tel que mentionné lors d’un travail pratique précédent, si une information est manquante, la catégorie ou le type d’information ne figure tout simplement pas sur la notice. Aucun espace vide ne s’y trouve, de sorte qu’un utilisateur pourrait malheureusement ne pas se rendre compte d’une absence quelconque, ne sachant pas que la donnée en question est recensée pour d’autres objets, par exemple.

Cependant, plusieurs lacunes pourraient être soulevées par les rédacteurs de la norme SPECTRUM : Effectivement, bien que TPT inclue au sein de ses courtes descriptions des références bibliographiques et associe à toute image un statut de droits d’auteurs, couvrant quelques aspects de la bonne pratique, les informations quant au statut légal et physique de l’objet, comme son propriétaire, son emplacement, la personne responsable de la documentation, etc., ne sont pas disponibles. Il serait donc complexe d’identifier des changements d’informations survenus comme les contributions des propriétaires originaux, les historiques des modifications ou les dates de documentation, qui n'y sont pas affichés. 

En revanche, Te Papa Tongarewa rend disponibles certaines informations que SPECTRUM survole très brièvement dans sa politique sur le catalogage, comme des synthèses narratives particulièrement complètes, des catégories iconographiques telles que « depicts » et « about », et des cartes et taxonomies interactives, qui permettent au public de faire une exploration complète de l’objet en question.

Je crois donc que les différences identifiés ci-haut ne reflètent pas une qualité moindre des métadonnées présentées par Te Papa par rapport à la norme SPECTRUM, mais plutôt un objectif différent. Le musée priorise l’accessibilité aux données culturelles, et non l’affichage et la conservation de données à des fins préventives (légales et éthiques) ou à des fins de gestion interne.

## 29 septembre

Anne-Julie: Cloche [Traduction libre anglais vers le français]
Numéro de l’objet : 925.26.170
Géographie : China
Nom de l’objet: Cloche
Date : 771-221 BC
Période : Dynastie Zhou de l’Est
Technique : bronze coulé
Mention de source : Bishop William C. White Collection
Collection : Chine
Département : Arts et culture : Chine
Emplacement dans la galerie : pas exposé

Commentaires: 
Si l’on suit les normes Spectrum, la méthode de catalogage de la section Arts et culture de la Chine du Royal Ontario Museum gagnerait à être revisitée et enrichie sur plusieurs plans.
Plusieurs informations essentielles concernant l’identification de l’objet, son contexte historique, sa collecte sur le terrain et sur sa production ne figurent pas sur la fiche. Par exemple, ni les dimensions, ni les caractéristiques distinctives de cette cloche, ni le peuple et/ou culture associée, ni même son lieu de provenance ne sont précisés. Le site archéologique d’où elle provient n'est pas mentionné, pas plus que la province où elle aurait été acquise. Cette absence d’information est potentiellement dû au fait qu’une grande partie des artéfacts acquis en Chine par Bishop White, l’un des principaux contributeurs de la collection, a été achetée auprès de particuliers, certains ayant même été introduits illégalement au Canada (Dong 2005). 

Ce manque d’information est d’autant plus problématique que plusieurs autres objets de la collection partagent le même nom générique de « Bell », eux aussi dépourvus de toute indication relative à leur provenance ou à leur contexte sociohistorique.  Toutefois, l’absence de contextualisation n’est pas un phénomène généralisé à l’ensemble de la collection du ROM, puisque plusieurs autres objets archéologiques bénéficient d’une brève description dans leur fiche en ligne.

Enfin, la fiche ne contient pas non plus aucune référence concernant son élaboration. Nous ne savons pas qui est l’auteur.ice et/ou l’éditeur.ice de la fiche. Il en est de même pour sa date de publication. 

Je vous ai envoyé mon travail par courriel car mon tableau ne voulait pas coller sur le Framapad.  Désolé.

Ema : El 3 de Mayo, Goya
Numéro : P000749
Nom de l'objet : peinture
Artiste : Francisco de Goya y Lucientes. 
Courte description : Le 3 mai 1808 à Madrid de Francisco de Goya (1814, Musée du Prado) représente l’exécution d’insurgés espagnols par les troupes napoléoniennes. Au centre, un homme en chemise blanche, les bras levés, incarne le martyr et la résistance. La lumière crue d’une lanterne oppose les victimes, vulnérables et expressives, à l’anonymat mécanique des soldats. L’œuvre dénonce avec force la brutalité de la guerre et est considérée comme un manifeste précurseur de l’art moderne
Emplacement actuel : Planta 0, Sala 064, Museo del Prado
Note précisant qui a consigné cette information et quand : inconnu, modif. 19-02-2025
Autres numéros de référence historique : Museo Real de Pinturas a la muerte de Fernando VII, 1834. Núm. 176.
DEPÓSITO GRANDE ESCUELA ESPAÑOLA / Ciento setenta y seis. LAs Víctimas de la noche del día 2 de Mayo de 1808 / D. Francisco Goya / Lº / 8.900
Inv. Real Museo, 1857. Núm. 1850.
Catálogo Museo del Prado, 1872-1907. Núm. 735.
Catálogo Goya, Pierre Gassier y Juliet Wilson. Núm. 984.
Titre : El 3 de mayo en Madrid o "Los fusilamientos"
Date : 1814
Contenu - évènement : Le 3 mai 1808 et l’exécution d’insurgés espagnols par les troupes napoléoniennes.
Dimensions : Height: 268 cm; Width: 347 cm
Matériau : Canvas et huile
Technique : Oil 
Sexe : masculin 
Style : ESCUELA ESPAÑOLA
Note sur l'historique de l'objet : Royal Palace, Madrid, 1814; entered the Prado Museum before 1834, registered in the ‘Large Deposit’ in that year; seen in 1840 by Théophile Gautier in the rooms of the Museum–described by the same author in 1843–; in 1850, by Count Clément de Ris; in 1867, it appears in the monograph on Goya by Charles Yriarte; it is finally registered in the catalogue of the Museum in 1872

Camila: Carte stéréoscopique de la Royal Insurance Company
No d’accession : 2010.44
Nom : Carte stéréoscopique
Description : Carte stéréoscopique présentant des photographies du bâtiment de la Royal Insurance Company, actif de 1860 à 1950, situé à Montréal. Ce bâtiment a précédé celui du musée Pointe-à-Callière, dédié à l’archéologie et à l’histoire de Montréal.
Emplacement actuel : Collection Pointe-à-Callière 
Date : 1er quart du 20e siècle, 3e quart du 19e siècle
Matériaux : papier
Technique : collé
Dimensions : 8,8 x 17,6 cm
Donateur : Denise Robert
Commentaires: La photographie stéréoscopique prend de l’importance au tournant du 20e siècle au sein des milieux bourgeois occidentaux. Cette technique, qui peut être considérée comme l’ancêtre de la 3D, consiste à donner une impression de relief et de profondeur au cerveau humain qui observe simultanément, à l’aide d’un stéréoscope, deux photographies distinctes et côte à côte représentant une même scène. Cette impression de relief est rendue possible par la différence de perspective de chacun des deux yeux sur un même objet.
Sur cette carte, on aperçoit l’édifice occupé par la Royal Insurance Company à partir du début des années 1860 et acquis par la suite par le gouvernement fédéral pour les douanes. De forme triangulaire, il est l’œuvre de l’architecte anglais John Williams Hopkins. La tour, munie d’une horloge, sert de point de repère à proximité du port, à une époque où le trafic maritime et ferroviaire était intense dans le secteur. Démoli en 1951 à la suite d’un incendie, ses fondations sont mises à jour à la suite des fouilles archéologiques qui ont précédé la construction du musée Point-à-Callière, qui occupe aujourd’hui ce site qui est également le lieu de fondation de Montréal.
Notes sur la qualité des métadonnées : Les informations présentées sur la page sont toujours uniquement pertinentes à l’objet présenté et ne donne que les informations qui sont connues. Dans le cas de cette carte stéréoscopique, le fabricant semble être inconnu car il n’est pas indiqué dans sa fiche, alors que cette information est donnée pour d’autres objets. 
Dans certains cas cependant l’inclusion de certaines métadonnées semblent arbitraire. C’est le cas lorsque l’on compare les fiches des différentes radios faisant partie de la collection. Sur certaines fiches il est indiqué le matériau alors que pour d’autre non. 
De plus, la fiche de certains objets, tel que la carte stéréoscopique en question, contient un paragraphe de contexte historique, indiquant pourquoi cet objet est intéressant dans le contexte de la collection ethnohistorique du Musée.  
Il n'y a aucune information sur l'auteur de la fiche mais certaines fiches nomment le photographe. 

Simon : 
    Objet 1 :  https://www.si.edu/object/knm-wt-15000a-knm-wt-15000-turkana-boy-human-fossil:nmnheducation_13109587
    Objet comparé : https://www.si.edu/object/kabwe-1-fossil-hominid:nmnheducation_11043697

Numéro d’objet  : (USNM # - United States National Museum) : EO401764 

    -          Fait usage de lettres, pas souhaitable. EO est pour ‘’education and Outreach’’. Identifie la collection. Les distinguerait des specimens originaux

    -          Les objets "EO" sont généralement conservés dans des espaces accessibles au public ou utilisés pour des activités éducatives, plutôt que dans des réserves scientifiques restreintes.


Nom de l’objet  : KNM-WT 15000A, KNM-WT 15000, Turkana Boy, Human Fossil

    -          Très large description

    o   KNM-WT 15000A = Code d’identification scientifique du fossile original

    §  KMN = Kenya National Museums (fossile original découvert au Kenya, y est enregistré dans sa collection)

    o   WT = West Turkana = Une region fossile à l’ouest du lac Turkana, nord du Kenya (Afrique de l’est)

    o   15000 = Numéro d’inventaire du spécimen original

    o   A = Partie spécifique du fossile original (crâne vs le reste du corps découvert).

    o   La partie sans le A désigne le spécimen complet. Donc on le lit comme ‘’crâne du Boy, Boy, Nom commun, type d’objet’’.


Nombre d’objets  : 1

Courte description :  ‘’ This object is part of the Education and Outreach collection, some of which are in the Q?rius science education center and available to see.’’

    - N’est pas descriptive de l’objet en tant que tel, sinon qu’il fait partie de x collection. N’est pas très utile pour l’identifier à des fins d’inventaires.


Emplacement  : Pas d’emplacement identifié dans le catalogue

Note de qui a consigné l’info et quand :   ‘’ Record Last Modified :1 Nov 2023’’

    - Pas de nom de qui a modifié la fiche

    - Date est correctement écrite : ‘’ jour en chiffre, mois, année en 4 chiffre’’.


Catalogage : Autres informations (non obligatoire, mais pertinentes)
 
Commentaires : notes exhaustives sur : 

    -  Couleur

    - Provient du squelette du Turkana Boy

    - Importance scientifique du Turkana Boy

    - Description physionimie (pelvis = mâle, dents = pas adulte)

    - Taille du crâne moulage

    - Homo Erectus

 
Caractéristiques distinctives
 

     Âge (Geologic Age) [SG1] : 1.6 mya

    Couleur[SG2]  : dans la description : ‘’Light beige …’’

    Matériau[SG3] x : ‘’Plastic, Paint’’

    Phase : dans la description : ‘’Light beige …’’

    Sexe : dans la description ‘’ male…’’.

    Date collecte terrain : 1984

    Chercheur sur le terrain : K. Kimeu

     

 
- Pour le spécimen étudié, ces informations ne sont pas catégorisées, mais écrits textuellement. L’info est là, relativement facilement accessible, mais manque de standardisation. 


Jade : 
Objet sélectionné : https://www.museedelaguerre.ca/collections/archive/3182135 
Informations de base (identification)

    Numéro d’objet : 19930065-524 (acquisition), O.3750 (numéro de l'image), CCO-CWM-FWWWP-188-EO-3750 (numéro de CD), 5605-2057-25R3-EO-3750 (Numéro barcode du CD)

    Nom de l’objet / titre : 12" Naval Howitzer in action = Un obusier naval de 12 pouces (30 cm) en action

    Nombre d'objets : 1

    Courte description : Photographie en noir et blanc montrant un obusier naval entouré de plusieurs artilleurs canadiens en uniforme

    Emplacement actuel : Archives iconographiques - Musée canadien de la guerre. Cote de rangement (1) : CWMMCG ARCH PHOTOS O.3750. Cote de rangement (2) : CWMMCG ARCH DIGITAL

    Propriétaire actuel : Musée canadien de la guerre

Informations sur l'identification

    Âge : 1917

    Couleur : Noir et blanc (non mentionné)

    Renseignements sur le contenu et le sujet :

    Contenu – activité : Artillerie en action (en guerre)

    Contenu – concept : Guerre, artillerie, transport militaire, "military railroads"

    Contenu – date : Novembre 1917

    Contenu – nom de l’événement : Première Guerre mondiale (1914-1918)

    Contenu – note : Photographie officielle canadienne prise pour documenter l’effort de guerre. Propagande?

    Contenu – type d’objet : Photographie (document iconographique)

    Contenu – peuple : Canadien

    Contenu – lieu : Europe (lieu exact non précisé)

    Dimension, y compris :

    Partie mesurée : Image au complet (tout le support)

    Valeur de dimension : 11.5 x 10 cm

    Unité de mesure de dimension : Centimètre

    Forme : Rectangulaire

    Matériau : Papier photographique (non mentionné, mais supposé)

    Style : Photographie documentaire de guerre

Informations sur l’historique et les associations

    Activité associée : Documentation de guerre

    Concept associé : Mémoire historique

    Date associée : Novembre 1917 (ou 1916–1919, activité du Canadian War Records Office)

    Date de l’événement associée : 1914-1918

    Nom de l’événement associé : Première Guerre mondiale

    Organisation associée : Canadian War Records Office (CWRO)

    Peuple associé : Canadien

    Personne associée : Max Aitken (Lord Beaverbrook), Captain Harry Knobel, Lieutenant Ivor Castle et Lieutenant William Rider-Rider

    Lieu associé : Europe/France

    Type d’association : Producteur / documenteur officiel

    Note sur l’historique de l’objet : Le CWRO a produit environ 7900 images (certaines sont mises en scène, mais la plupart sont documentaires)

Information de collecte sur le terrain : Non applicable
Information sur la production des objets

    Date de production de l’objet : Novembre 1917

    Organisation de production de l’objet : Canadian War Records Office

    Peuple de production de l’objet : Canadien

    Personne de production de l’objet : Lieutenant William Rider-Rider / Ivor Castle / Harry Knobel (photographes du CWRO, mais l’auteur exact est non précisé)

    Lieu de production de l’objet : Europe (probablement Front occidental - non mentionné)

    Raison de production de l’objet : Documentation officielle de guerre et/ou propagande? (non mentionné)

    Technique : (?)

Information sur la contribution du propriétaire : Non documenté
Information de référence : Non documenté
Historique des modifications (information sur les changements faits dans le catalogue) : Non documenté

Commentaire : En comparant la notice du Musée canadien de la guerre avec la norme Spectrum, on voit que plusieurs informations ne correspondent pas directement. Ils ne correspondent que partiellement aux catégories indiquées par Spectrum (ou est inscrit de manière différente). Spectrum insiste beaucoup sur la normalisation des termes (liste d'autorité), mais je ne crois pas que le catalogue analysé propose une telle normalisation et il manque d'organisation (selon moi). Les métadonnées du musée sont intéressantes pour comprendre l'histoire et contextualiser l'objet, mais elles manquent de précision technique pour être facilement partagées ou comparées avec d'autres bases de données (entre institution).

Jeanne : 
    
Œuvre choisie: https://ago.ca/collection/object/2006/84.1  
Les informations de bases:  

    Numéro d’objet unique : 2006/84.1 

    Nom de l’objet : Night, asleep in the Cabane from "Moose Hunting" Portfolio 

    Nombre d’objets : 7  

    Courte description (ou image) : photographie du portfolio “Moose Hunting” 

    Emplacement actuel : Pas actuellement exposé, mais disponible le mercredi de 1 à 4 h 30 au Centre d'études sur les impressions et les dessins 

    Personne responsable de la documentation et date de documentation :   

 
Information sur l’identification des objets 

    Age : 1866 

    Nom de l’objet : photographie 

    Catégorie : photographie 

    Technique : Tirage albumen 

    Mesures :  

Image : 10 x 13,2 cm (3 15/16 x 5 3/16e de pouce)  
Montage: 23 x 33,5 cm (9 1/16 x 13 3/16e de pouce.)  
Matière: 45,7 x 35,6 cm (18 x 14 pouces) 

    Acquisition (ligne de crédit)  : Achat, fonds donnés à la mémoire d'Eric Steiner et Anonyme, 2006 

La qualité des métadonnées :  
Les informations données sur la page de l’œuvre dans le catalogue en ligne sont  succinctes et courtes. Mais l’œuvre est rattachée à son portfolio et aux autres photographies présentent.  

Sandrine : 
    
Objet sélectionné : Collection specimens - Specimens - NHMUK013376586 - Data Portal
Information sur l’identification de l’objet :
·       Numéro d’objet unique : NHMUK013376586
·       Nom de l’objet : Anthene collinsi d'Abrera, 1980
·       Nombre d’objets : 1
·       Courte description : Spécimen de Anthene collinsi, de la famille Lycaenidae de l’ordre des Lepidoptera. 
·       Date de documentation : 2019-03-15T10:03:03+00:00
·       Autre numéro de référence : NHMUK:ecatalogue:8779351
·       Code de la collection : BMNH(E) (Entomology)
·       Sous-département : Lepidoptera
Information sur la description de l’objet : 
·       Date : 1980
·       Couleur : bleu, noir, brun
·       Source : don de P H. Lindsay
Information de collecte sur le terrain : 
·       Lieu de collecte : Éthiopie, Afrique
·       Coordonnées : 599.6138841m
Information de référence :
·       Références : Biodiversity Heritage Library, Catalogue of Life icon Catalogue of Life, GBIF
Historique des modifications : 
·       Date de documentation : 2019-03-15T10:03:03+00:00
·       Dernière modification : 2021-01-30T17:15:30+00:00
Commentaires sur la qualité des métadonnées proposées dans le catalogue étudié : 
Le catalogue ne présente pas certaines informations d’identifications pour l’objet choisi, tels les emplacements actuels des objets, la description des objets, les dimensions ou le propriétaire actuel. En comparant avec quelques autres spécimens de leur collection, il est apparent qu’il y a un certain manque de cohérence entre les différentes entrées du catalogue. Certains objets on davantage de données présentées, comme une courte description ou des informations relatives à la stratigraphie liée à la collecte de terrain. On ne spécifie pas non plus si les spécimens/objets sont actuellement exposés ou non. 


--------------------------------------------------------------------------------------------------------------------------------------

## 22 septembre

Suzanne:  Spectrum: Prêt d'objets

Jade : Soin et conservation des collections

La normes Spectrum

    Les grandes lignes ; la procédure de Soin et conservation des collections consiste à gérer et documenter tout travail de conservation/restauration effectué. Elle traite par exemple des traitements pour la dégradation, la réparation des dommages ou l’amélioration de l’apparence des objets.

    Au cœur de la gestion des collections.

Marche à suivre proposé (3 axes principaux) 
1. Consentement du travail de restauration (autoriser)

    Objectif ;  obtenir une autorisation écrite avant toute intervention

    Définir la porté du travail (ce que ça implique (accord) : quoi, pourquoi, comment)

    Calendrier

    Fournir les informations sur l'objet au restaurateur (numéro de l'objet, description, matériaux, historique des restaurations, etc.)

    Signer l’accord et l’archiver

    Consignation de l'information sur le travail de restauration

    Numéro d'objet (ou entrée)

    Numéro de référence du traitement de restauration

    Restaurateur

    Adresse

    Méthode

    Etc.

2. Réalisation du traitement de restauration (agir)

    Objectif ; effectuer les travaux en respectant les normes et selon une planification établie au préalable

    Transfert de l’objet

    Fournir au restaurateur les informations

    Réalisation du traitement

3. Consignation du traitement de restauration (documenter)

    Objectif ; documenter tous les détails 

    Avant : référence de traitement, restaurateur, date, etc.

    Après/pendant ; date, type de travail, intervention, matériaux utilisés et résultats

    Photo, rapport et recommandation

    Planification d’un suivi (date de rappel)

Liens avec les autres procédures ; 

    Les interventions de conservation sont directement liées à l’état des objets et à leur analyse technique parce qu’elles découlent souvent des constats établis (constat d’état et analyse technique) sur leur état et leur besoin de restauration.

    Cette procédure peut également être motivée par d’autres raisons comme le déplacement d’un objet :

    Contrôle des emplacements et des déplacements

    Emprunt d’objets

    Prêt d’objets

    Sortie d’objets

    Etc.

    Documentation et catalogage ; mise à jour du catalogue et intégration de toutes nouvelles informations obtenues du processus.

    « Consigner les détails relatifs au traitement, et le traitement effectué sur chaque objets  » (p. 8)

    Les restaurateurs participent également à d’autres procédures. Leurs analyses et leurs recommandations peuvent donc servir de base pour les travaux à suivre

*Le travail de restauration peut être demandé par « quelle que soit l’autre procédure Spectrum qui demandait le travail de restauration » (p. 7). Indique une large intégration des procédures et des liens qu’elles entretiennent entre elles.
Critiques/observations
Points forts : 

    La documentation est vraiment mise de l’avant

    Accent sur une analyse technique fait avant l’intervention (et non seulement le processus lui-même)

Limites : 

    Très général, absence de détails

    Suggestion : ajouter (si possible) une annexe ou section sur les protocoles scientifiques recommandés pour les analyses et les traitements 

    Biais institutionnel : semble s’adresser à des institutions qui ont accès à des ressources importantes. Les plus petites institutions pourraient trouver certaines exigences difficiles

    Vocabulaires techniques : le texte suppose que le lecteur connaît déjà des termes techniques et ça peut exclure les personnes qui ne sont pas spécialistes.

    Suggestion : Définir les termes techniques dans un glossaire ou une section autre


Jeanne : Constat d’état et analyse technique 

Sophie : Retrait d'inventaire et aliénation

Sandrine : Catalogage

Hugo:  Acquisitions et enregistrements

Ema : Planification des mesures d’urgence pour les collections

Anne-Julie: Reproduction

Camila: Utilisation des collections

Simon : Examen des collections



---------------------------------------------------------------------------------------------------------------------

## 15 septembre 

Prénom : Nom du musée + l'url du catalogue svp. 

Jade Sirois : Musée canadien de la guerre (https://www.museedelaguerre.ca/collections/)


Observation générale du site

    Le catalogue du musée est très accessible depuis une simple recherche sur le web. Depuis la page d’accueil du site, la section « Recherche et collections » est bien affichée en haut (ça facilite donc sa consultation). Je trouve que cette section est globalement bien intégrée au site. Il y a même une section « Objets vedettes de nos collections  » plus bas.

    Le site est offert en anglais et en français (favorise son accessibilité à un plus grand public).

Méthodes et modes de recherche

    Sur le catalogue, il y a plusieurs méthodes de recherche. La première est une recherche de base. Il y a aussi une méthode de recherche avancée. Celle-ci propose des filtres et divers critères comme la date, l’événement, le département ou encore le service. L’outil est assez complet.

    Après recherche, les artefacts et les archives sont présentés comme deux catégories distinctes (permet une meilleure organisation et facilite la recherche).

    Il y a aussi l’option de tri par ordre de classement (pratique si l’on a des préférences)

    Il est également possible d’affiner les résultats grâce à des filtres supplémentaires (disponibles à gauche du catalogue).

    J'apprécie l'affichage du titre de l'objets (ce n'est pas le cas pour d'autres catalogues de musées)

Présentation de l’objet

    Lorsqu’on sélectionne un objet, plusieurs informations sont disponibles à la consultation (entre autres le nom de l’objet, son numéro d’inventaire, la date de production, la catégorie, les matériaux utilisés et bien d’autres détails).

    La seule critique que j’aurais à formuler concerne le manque de descriptif (détaillé ou non) permettant de mieux comprendre l’objet (comme son contexte historique ou sa fonction). Une description serait un vrai plus! 

    Exemple : Ce pistolet a été utilisé lors de la bataille de Vimy en 1917, pendant la Première Guerre mondiale, par un soldat canadien.

    Outre les objets qui ne comptent pas de photo (et je me demande pourquoi), les photos des objets sont de bonne qualité et nous permettent de bien saisir les détails. 

    L’option d’agrandir, de rapprocher et de retourner l’image est offerte. C’est une fonction très pratique pour étudier l’objet.

    Lors de la consultation d'un artefact/d'une archive, on peut découvrir d’autres objets similaires en suivant le lien associé à ses caractéristiques (par exemple : « pistolet » pour la classification ou « armes et technologie » pour le département). 

    Aucune ressource supplémentaire proposée pour approfondir la compréhension de l’objet.


*En général, les données proposées par le catalogue en ligne sont bien présentées et faciles à trouver. La manière de présenter les informations est cohérente et uniforme.

Suzanne Desormeaux: Musée McCord Stewart à Montréal

    Le catalogue en ligne est facile à trouver. Les choix se trouvent en haut dans le menu principal. Le 4e onglet à droite est intitulé Collections et, en cliquant dessus, le deuxième choix est Online Collections. En cliquant sur Online Collections, nous avons sept choix : Archives; Documentary Art; Dress, Fashion and Textiles; Material Culture; Indigenous Cultures; Photography; and the Public Domain.

2. Les critères de recherche sont:  nom de l’objet, date, personnes, culture, ville, classification, division, credit, avec image et exposé.
3. Les informations relatives aux artefacts sont : créateur, période, médium / technique, dimensions, classification, origin , numéro d'accession, division, collection, crédit, achat, status.  Il y a aussi les informations concernant le copyright et l’usage sur la page.
4. Les liens et les rebonds sont : Classification, Division, et Collections. Il y a aussi un onglet Découvrir Plus, ainsi que des icônes pour partager et pour obtenir la page PDF avec la photo et les informations.
5.  L’information est éditorialisée par les résultats de nouvelles recherches, et aussi par l’information du public (à vérifier bien sûr). L’information suivante se trouve sur la page de collection.  "L’information sur les objets de nos collections est mise à jour afin de refléter les résultats de nouvelles recherches. Si vous avez des renseignements au sujet de cet objet à nous communiquer, veuillez faire parvenir un courriel à reference.mccord@mccord-stewart.ca."
6.Les informations données montrent une accessibilité au public général. Les informations ne sont pas trop scientifiques ou difficiles à comprendre et la collection est facile à explorer. Le musée en ligne McCord Stewart montre aussi un intérêt pour la participation du public grâce à la demande d’information, ainsi qu’un statut non statique puisque de nouvelles recherches sont mises à jour.

Anne-Julie Robitaille: Collection art et culture de Chine du Royal Ontario Museum https://collections.rom.on.ca/en/groups/china/results
1. Choix :

    Le ROM possède la plus grande collection archéologique de Chine en Amérique du Nord

    Une très grande partie des artefacts archéologiques ont été collectés par des missionnaires Canadiens, relatant ainsi de la profonde histoire entre les différentes institutions du Canada et de la Chine ainsi que des dynamiques sociopoitiques entre leurs différents acteur-ices

    La collection couvre plusieurs époques, allant du Néolithique à l’époque moderne, et une très grande variété de matériaux (céramique, lithique, jade, bronze, murales de bois, peintures, etc.)

2. Exploration du catalogue:

    Disposition de chaque artéfact facilitant l’exploration de la collection et permettant le « flânage »

    Chaque fiche contient le titre de l’objet et son lieu d’origine (les matériaux ne sont pas indiqués)

    Les titres en chinois optent pour l’écriture traditionnelle

    Incohérence dans les informations affichées dans leur catalogue:

    Certains titres sont offerts en anglais et en chinois, alors que d’autres sont seulement affichés en anglais

    Il en est de même pour les lieux d’origine (ex : China vs China 中国)

    Les titres d’œuvres en chinois utilisent l’écriture traditionnelle, mais le nom des lieux est en caractères simplifiés

    Seulement une partie des objets ont leur date et/ou période historique incluse

    Les objets de la collection ne sont pas organisés dans un ordre particulier

    Sur un même page, on y retrouve des objets de différents matériaux, différentes époques, différentes fonctions et différentes régions

    Les items peuvent disposés de différentes façons (images, listes, tables, carte) et en ordre différents selon:

    Pertinence

    Titre (A-Z)

    Date (le plus ancien)

    Numéro de l’objet (croissant)

    Fabricant principal

    Dernière mise à jour (croissant)

3. Recherche:

    L’interface offre une série de filtres organisés en 4 grandes catégories qui ensuite se sub-divisent en plus petites catégories (classification, département, pays, localisation géographique)

    L’interface ne permet pas de sélectionner plusieurs filtres en même temps. Ceux-ci peuvent s’additionner afin de préciser notre recherche, mais l’utilisateur-ice doit les sélectionner individuellement 

    Les titres de localisation géographiques se répètent sous différentes étiquettes ce qui alourdit la recherche (ex : Beijing, China vs Beijing (Peking China)

    Il en est de même pour les pays (ex : CHINA vs China)

    La classification d’objet contient différentes catégories mélangeant fonction, matériaux, provenance ce qui rend la recherche confuse

    Un même objet peut appartenir à plusieurs catégories à où regarder?

    L’interface offre seulement une barre de recherche générale à tout le catalogue du ROM sans faire de distinction selon les différentes catégories

    L'interface n'offre pas de lien vers d'autres items ou autres informations (ex: période historique, région, matériaux, etc.)

4. Description des objets

    Chaque objet est accompagné d’une fiche contenant :

    Location dans la galerie

    Medium (matériaux)

    Géographie

    Période 

    Dimensions

    Numéro de l’objet

    Collection

    Département

    Bibliographie

    La profondeur des explications varie selon les objets. 

    La description peut inclure :

    Description et explication générale de la catégorie d’objets (ex : Paper gods)

    La fonction de l’objet et son contexte culturel, social et historique

    Une description plus spécifique à la collection du ROM (ex : combien d’objets de la même catégorie le ROM possède)

    Offre des suggestions de lecture si l’utilisateur-ice veut en connaître davantage sur le sujet.

    Mais n’incluent pas nécessairement un lien vers la publication. Il en incombe à l’utilisateur-ice de faire ses propres recherche

    Inclus le courriel du musée si l’utilisateur-ice désire faire part d’une information erronée 

    Quelques incohérences :

    Certains objets sont photographiés d’un seul angle alors que d’autres sont photographiés selon plusieurs angles

    Les dimensions de certains objets incluent seulement 2 dimensions sans les mentionner (ex : 2.8 x 2.2 cm)

    Credit Line pour seulement certains objets 

    Certains objets sont accompagnés d’une description exhaustive alors que d’autres n’ont que quelques lignes descriptives composées de phrases incomplètes


Jeanne Beaudonnet : Art Gallery of Ontario (https://ago.ca/) 
Le catalogue en ligne se trouve dans l’onglet “Art & Artist” sur la page d’accueil du site du musée. Une fois l’onglet ouvert, on trouve différents accès possibles : Collections puis Collections, The Thomson Collection, Collections in focus, Conservation. La page “Collections” du musée est composé de sous-catégories, par exemple : collection d’art canadien, européen, autochtone. 
Puis une fois sur la page “Collections”, la page d’accueil montre un texte qui explique les collections et un autre lien permet d’accéder au “Browse the collections”, de parcourir la collection. Le lien permet l’accès à une autre page avec une propositions d’artefacts et des critères de recherche plus précis comme le nom de l’objet, le type d’objet, par période etc.  
Une option qui permet de comparer les objets de la collection, mais elle ne fonctionne pas correctement pour le moment.  
Les artefacts sont photographié en haute définition, s’il est numérisé. Les pages possèdent peu d’informations sur l’artefacts, seulement des informations essentielles. Chaque page se présente avec : Nom de l’objet, catégorie, date, le médium, ligne de crédit, numéro d’inventaire, location, numéro de la galerie, taille, signature (si signé), et une liste de nom reliant le sujet de l’artefact à d’autres artefacts de la collection. Un lien est aussi visible pour accéder à une demande de droit d’utilisation des images du musée.  
Le musée explique ses collections dans les grandes lignes et mettent l’accent sur certaines pièces importantes de leur collection avec “ Collections in focus”, avec par exemple “the boxwood project”. Pour avoir plus d’informations sur les collections, il existe des catalogues imprimés. Ils utilisent leur collection. Et le musée accorde une place aux conservateurs du musée avec une page dédiée.  


Ema Holgado : Museo del Prado
- J’ai choisi ce musée car je le trouve particulièrement beau ; son catalogue en ligne est riche. De plus, vous allez le voir, mais les informations disponibles sur le catalogue sont particulièrement riches et détaillées ce qui met en confiance quant à la transparence et l’envie de partage du musée à propos de ses collections. 
 En entrant sur le site, le musée nous propose l’achat de son catalogue papier pour 35,58 euros. Un onglet « Obras » nous permet tout de même d’avoir accès à une partie du catalogue en ligne. Nous prendrons l’exemple de l’œuvre « Penitent Magdalene ».
Sur les différentes pages des œuvres, il est possible de retrouver une image de bonne qualité sur laquelle il est possible de zoomer. Ensuite, on trouve le nom du peintre, la date, le support et la technique (ex. : huile sur toile), ainsi que le lieu où l’œuvre peut être vue dans le musée. Sous cela, un texte d’interprétation nous permet d’en savoir plus sur l’œuvre et propose des liens vers des événements historiques cités ou des termes techniques (ex. : eucharistie, Inquisition, Concile de Trente, etc.), puis la source du texte.
En bas du texte, un lien nous permet d’accéder à une frise où sont placées toutes les œuvres présentées dans le catalogue, afin de pouvoir les situer dans le temps les unes par rapport aux autres, mais aussi par rapport au contexte historique indiqué sur la frise. Il s’agit d’une manière particulièrement intéressante de proposer une mise en contexte de l’œuvre.
À gauche, une indication nous donne plus d’informations sur le peintre et sur sa vie, tout en proposant un lien vers sa fiche technique. À droite, des « tags » indiquent l’année de l’œuvre (1583), ses caractéristiques techniques (oil, painting), des éléments présents dans l’œuvre (skull, crucifix), et renvoient à d’autres œuvres du catalogue ayant les mêmes « tags » ou les mêmes caractéristiques. Par la suite, des liens vers des vidéos où apparaît l’œuvre nous sont proposés.
Nous avons ensuite accès à une section « Technical data » ou « Ficha técnica », qui nous donne le numéro d’inventaire, l’auteur, le titre, la date, la technique, le support, les dimensions et la provenance. Le travail est transparent et très bien décrit. Une photo de l’œuvre sans et avec son cadre est aussi proposée. Ensuite, des menus déroulants nous permettent d’accéder à la bibliographie de la fiche, à d’autres inventaires, aux expositions où l’œuvre a été présentée, à un plan du lieu où se trouve l’œuvre, ainsi qu’aux inscriptions présentes sur l’œuvre (ex. : « M·D·L X·XX III » Dated. Front, left side. « N.o 90 Magdalena oratorio de la R.a » Inscribed in pencil. Frame, back, upper bar). Il est aussi possible de savoir quand la fiche a été modifiée et quand elle a été créée.
Enfin, d’autres œuvres en lien nous sont proposées, comme des lithographies de l’œuvre par d’autres artistes, avec déjà des liens vers les lithographes, les directeurs et les imprimeurs. Cela est suivi, en bas de page, d’un carrousel d’autres œuvres peintes par l’artiste, à consulter.

Hugo Barsacq-Camard: Musée du Quai Branly (÷https://collections.quaibranly.fr/)
 
Le catalogue des objets est affiché sous l’onglet des collection. Ce meme onglet regroupe d’autres liens comme des projets en lien avec certaines collections ainsi que des informations sur diverses fonctions dans le musée.
critères de recherche offerts
Les critères de recherche sont organisés selon diverses catégories qui peuvent être cumulées pour mieux filtrer. Par exemple, on peut rechercher selon des types d'objets (films, textiles, photographie, instruments, etc.), mais aussi selon les cultures et les régions. Ces dernières sont subdivisées pour former une hiérarchie qui devient de plus en plus précise, tandis que le nombre d'objets se réduit (par exemple : Asie - Asie septentrionale - Russie - District Fédéral du Sud - Province de Volgograd). Les cultures, par contre, sont énoncées selon 5 régions continentales (Asie, Océanie, Amérique, Europe, Afrique). Chaque filtre va aussi réduire les options visibles concernant les autres filtres, ce qui peut aider à la recherche. Il y a aussi une carte du monde qui démontre combien d'objets proviennent de chaque continent et de chaque pays, ainsi que l'option de filtrer pour voir seulement les objets exposés.
informations relatives aux artefacts
La majorité des objets ont une ou plusieurs images qui peuvent être agrandies ou réduites, et certaines sculptures ont des images de chaque angle. On retrouve des informations typiques d'un cartel : titre, dates, lieu, culture, matériaux, numéro d'inventaire, date d'acquisition (s'il y a lieu), et certains objets ont une petite description ou des informations en lien avec l'usage de l'objet. Les œuvres d'art indiquent l'artiste, même si une grande partie semble être inconnue ou anonyme. Les descripteurs de chaque objet agissent comme des liens url qui regroupent chaque objet. Par exemple, en cliquant sur le nom du donateur, tous les objets donnés par celui-ci sont affichés. De même pour les matériaux utilisés, l'endroit de production, l'artiste, etc. Ceci permet aussi de voir combien d'objets ont une acquisition indéterminée.
Le musée démontre une grande sélection d'information accessible au public. Cependant en ce qui concerne les objets, on retrouve peu d'informations sur l'histoire de l'artefact lui-même (plus orienté sur les catégories ou de manière générale), et les cultures ou les régions ne vont pas avoir de descriptifs.

Sandrine Dufour : Natural History Museum (UK) ( Collections | Natural History Museum ) 
Accès au catalogue en ligne : 
Le catalogue du Natural History Museum se retrouve dans l’onglet Our Science, qui regroupe le département de la recherche, les collections, ainsi qu’un répertoire des experts et expertes de l’institution. Sur la page principale du Musée, l’onglet des collections n’est pas immédiatement apparent, il faut se rendre dans l’onglet Our Science afin de trouver le lien vers les collections. Après avoir accédé à la page générale des collections, nous nous retrouvons devant sept premières sous-catégories, divisant leur collection par discipline scientifique (collections d’entomologie, de botanique, de zoologie, de paléontologie, de minéraux, de spécimens moléculaires et d’archives). Par la page générale des collections, il est également possible d’effectuer directement une recherche pour un spécimen spécifique. Selon la discipline scientifique choisie, une autre série de catégories sont proposées, afin d’organiser les collections. Des informations générales sont présentées à propos de ces sous-catégories de collections. Enfin, il est important de noter que les collections en ligne ne sont pas accessibles directement par le site web du Musée, il faut suivre un autre lien vers le Data Portal, un site web regroupant les collections et données de recherches du Natural History Museum (Welcome - Data Portal) .
Critères de recherche : 
Différents modes de recherches sont proposés via le Data Portal. Sur la page d’accueil, une barre de recherche permet de chercher un spécimen spécifique parmi les spécimens, les collections, ou tous les résultats. Ce site web propose également une banque d’images de spécimens de leur collection. Dans cet onglet, des filtres peuvent être ajoutés afin de faciliter la recherche : mot clé, taxon, type, type d’image et source. Plusieurs filtres peuvent être combinés dans cette recherche.
Informations présentées : 
Une fois qu’un objet est sélectionné dans le catalogue en ligne, une image de l’objet est présentée, accompagnée d’une fiche. Cette fiche contient le numéro de catalogue de l’objet, sa description, le type de collection d’où il provient, la classification du spécimen (règne, classe, ordre, famille, genre, espèce), son nom scientifique, ses dimensions, ainsi que les liens vers l’image de l’objet (avec la référence du droit d’auteur de l’image). 
Liens entre les artefacts :
L’interface de recherche ne permet pas d’ouvrir plus d’un objet à la fois, afin de réaliser des comparaisons. Cependant, les filtres de recherche permettent de faire ressortir des objets similaires. Les résultats de recherche sont présentés sous forme d’image avec un titre descriptif, il est donc possible d’effectuer de simples comparaisons par un premier balayage visuel. Lorsqu’un objet est sélectionné, l’interface de recherche ne propose pas d’objets similaires, il y a seulement la fiche descriptive de l’objet sélectionné.
Présentation des contenus : 
Le Data Portal semble davantage être un outil de recherche pour des individus ayant déjà des connaissances sur les collections présentées, que pour des individus non-informés. Les filtres de recherche requièrent des termes spécifiques associés aux objets recherchés (par exemple, le rang taxonomique, le nom du genre ou de l’espèce recherchée). De plus, les informations relatives aux objets sont présentées sous forme d’une liste, sans vulgarisation scientifique, support visuel ou autres outils pour faciliter la compréhension. 
Discours du Musée : 
Le catalogue en ligne du Musée montre l’ampleur de leur collection, leur page d’accueil exprime d’emblée que 6 055 472 spécimens de leur collection sont accessibles par cet outil de recherche. On comprend d’ailleurs que ce musée doit regrouper une équipe d’experts et expertes de plusieurs disciplines des sciences naturelles, par la variété des spécimens présentés. Sur son site web, le Natural History Museum se définit comme étant un centre de recherche d’importance mondiale, le Data Portal permet en effet d’accéder à des recherches de plus de 1000 scientifiques. Un onglet de ce site web explique également comment citer les articles scientifiques ou les objets présentés en ligne. Le catalogue en ligne présente des informations factuelles liées aux spécimens, qui semblent davantage être pertinentes pour des recherches scientifiques que pour la simple contemplation de leur collection.

Camila Maghraoui : Pointe-à-Callière (https://pacmusee.qc.ca/fr/collection/)
Le catalogue est accessible à partir d’un onglet disponible dans l’en-tête du site web en français et en anglais. On peut s’y rendre de la même manière que lorsqu’on souhaite voir la liste des expositions en cours ou pour l’achat de billets. Une fois sur la page Collections, le catalogue est divisé en deux collections : la collection ethnohistorique et la collection archéologique. Les objets dans la collection archéologique font partie d’une base de données partagée Réseau canadien d’information sur le patrimoine : Artéfacts Canada. Le Musée Pointe-à-Callière a déposé plus de 3800 fiches techniques numérisé sur cette base de données. L’information est aussi disponible dans la base de données d’Archéolab, qui semble aussi être partagée. La collection ethnohistorique est disponible sur un site web du Musée, c’est donc pour cette raison que je me concentrerai sur celle-ci. 
Il y a une barre de recherche au-dessus de la page, ainsi que l’option pour faire de la recherche avancée. Il est possible de faire de la recherche avancée à partir du Nom, Collections, Mots clés, Fabricant/Artiste, Matériaux, Période, Thématique, License d’utilisation. Il y a aussi des cases pour option « Avec image », « Avec un contexte historique » et « Exposé au musée ». Les options pour effectuer une recherche à l’aide du Numéro d’accession, Date de début et Date de fin sont aussi présentes. Finalement, sur la page d’accueil du site des collections il y a différents objets Coup de cœur, l’option d’Explorer les collections par thématique ou par période. 
Lorsque l’on sélectionne la fiche d’un objet, celle-contient toujours une brève description, son numéro d’accession ainsi que l’option de télécharger la fiche en PDF. Puis, tout dépendamment de l’objet et des informations connues : des images, les mêmes informations qui sont retrouvables par la recherche avancée, son contexte historique ainsi que des informations sur le droit d’auteur et sa localisation s’il s’agit d’objets d’archives. Lors de la recherche traditionnelle, il y n’y a aucun lien entre les fiches, chaque artéfact est considéré individuellement. Il n’est donc pas possible de faire des rebonds entre les différentes fiches sans retourner dans la recherche ou dans les catégories d’explorations offertes par le catalogue. Pour les artéfacts faisant partie d’une collection, il est possible de voir une liste de tous les objets dans cette collection, ainsi qu’un carrousel au bas de la page invitant les visiteurs à Découvrir plus, généralement des artéfacts similaires ou du même type. 
Au bas de chaque fiche il est marqué : « Les informations sur les objets proviennent de notre base de données qui a été bonifiée au fil des années. Si vous avez des renseignements sur cette pièce, n’hésitez pas à nous écrire afin de nous en faire part. » invitant donc plus d’informations de la part des visiteurs ainsi qu'un intérêt à obtenir plus d'informations ou même des corrections. Avec l’option de recherche Exposé au musée, il est facile de retrouver des pièces qui auraient pu piquer l’intérêt d’un visiteur et de pousser sa recherche à l’aide des artéfacts qui lui sont liés dans sa fiche. 


Simon Gravel : National museum of natural history (Smithsonian) - https://www.si.edu/collections

En explorant les différents catalogues proposés par les musées d’histoire naturelles, celui du Smithsonian aura su accrocher mon intérêt. Bien mis de l’avant dans l’onglet ‘’Explore’’ du site web, le catalogue semble faire partie intégrante de la présentation virtuelle du Musée.
On remarquera de prime abord que l’introduction même du catalogue, à savoir la page précédant l’outil de recherche, est elle-même riche d’informations. En cliquant sur le lien fourni plus haut, on remarque en effet dans cette page web un préambule au catalogue, un avant-goût, qui permet un coup d’œil rapide sur la diversité de la collection. 
D’abord présentant les principes de ‘’digitalisation’’ et de conservation du musée est offerte sous forme d’articles et de capsules vidéo, en lien externe. Cette pratique ouvre la porte au grand public de l’arrière-scène du musée, et lui offre à voir son fonctionnement et les acteurs rendant possible la richesse du catalogue numérique. 
Sur cette même page introductive, maintenant plus bas, on y retrouve la section ‘’Collections Sampler’’, donnant à voir de multiples objets à références populaires : le chapeau d’Abraham Lincoln, le module de commande d’Apollo 11, la poupée Kermit the Frog, une réplique de crâne de tricératops… Cette approche guide sans détour le regard, accroche immédiatement l’intérêt : elle interpelle différents types de visiteurs, qui reconnaîssent alors sans nul doute le symbolisme d’au moins un de ces objets. C’est une astuce ingénieuse : la diversité des thèmes, et la familiarité des références suffit à accrocher le visiteur, et à l’entraîner dans le catalogue principal. On accède à ce dernier en haut de page, en cliquant sur ‘’Just browsing’’.

En accédant au catalogue, on se retrouve devant plus de 26 millions résultats répartis parmi 2 onglets généraux et 5 onglets spécifiques. Les onglets généraux, ‘’Top Results’’ et  ‘’All Digital Records’’ renvoient respectivement à un aperçu populaire et à un recensement complet. Parmi ceux plus spécifiques, les onglets ‘’Website’’ et ‘’Exhibitions’’ présentent différents événements et articles en cours au musée; alors que  ‘’Collection Images’’, ‘’Collection Sets’’, et ‘’3D Assets’’ renvoient à différents moteurs de recherches, chacun ayant son propre point de focus. 
Je me suis particulièrement attardé aux onglets ‘All Digital Records’’ et ‘’3D Assets’’. 
L’onglet ‘’All Digital Records’’ offre une multitude de filtres de recherche, dont par exemple le département d’affiliation de l’objet, le type de média, le sujet, la date de l’objet, la culture etc. Les objets qui constituent cet onglet sont figurés par une série d’images, affichés sous forme de grille. Ces images représentent tantôt l’objet même, tantôt son recensement historique (une photo de sa description dans le catalogue historique, voir cet exemple). 
Cliquer sur un objet nous offre une fiche descriptive relativement standardisée : entre autres, une description sommaire de son contexte, de sa signification, ou de son aspect physique, la date d’acquisition de l’objet etc. Ces catégories fluctuent légèrement selon le type d’objet.

À travers l’onglet ‘’All Digital Records’’, le visiteur entre peu en interaction avec la galerie, sinon par l’entremise des catégories claires et stratégiques. Cette manière de présenter la collection exige du visiteur de savoir ce qui l’intéresse. Elle décourage le déambulement immotivé, rêveur, d’une visite impromptue. Loin d’être un défaut, cette présentation mécanique semble bien contraster l’aspect justement déambulatoire de l’introduction à la collection, décris plus haut dans ce rapport. Elle informe sur les objets retrouvés dans le catalogue, point barre.
Un dernier arrêt nous amène à l’onglet intitulé ‘’3D Assets’’, qui lui, propose une manipulation virtuelle de plus de 3000 objets; crâne de gorille, porcelaine, vêtement, on y trouve de tout. Bien que les fiches informatives ressemblent à celles retrouvées dans l’onglet ‘’All Digital Records’’, le rapport individu-objet n’en est plus un strictement profane, cloîtré; plutôt, on devient acteur même dans l’apprentissage, jouant de notre curiosité, en exploration de tous les profils possibles. 

Le musée du Smithsonian semble donc endosser différentes stratégies de médiation à travers son catalogue. Alors qu’il accroche d’abord le regard par ses références populaires, il permet la flânerie et la découverte immotivée avec l’introduction de son catalogue. À travers les principaux onglets du catalogue même, on retrouve l’aspect typique de recensement d’un inventaire, lequel offre un moteur de recherche semi-personnalisé à l’aide des filtres proposés. Finalement, la visualisation 3D de certains des objets de la collections appellent à l’interaction avec les collections, et à un investissement bonifié du visiteur dans ses découvertes. 

Sophie Fox-Mauffette : Te Papa Tongarewa (Museum of New Zealand) - https://collections.tepapa.govt.nz/

Pourquoi avoir choisi ce musée ?

J’ai un intérêt marqué pour la Nouvelle-Zélande, comme j’aimerais un jour y étudier ou y travailler. Comme Canadienne et Québécoise, je trouve qu’il est très pertinent d’explorer des cultures et des pays avec une histoire coloniale semblable au Canada, et de découvrir comment les institutions de cette région intègrent des espoirs de décolonisation aux pratiques muséales locales. J’aimerais m’en inspirer, pour ensuite aider et guider les collections canadiennes lors de leur processus homologue.

Comment le catalogue en ligne s’intègre-t-il au site du musée ?

Le catalogue de Te Papa Tongarewa sert en même temps d'outil documentaire interne et d’opportunité pour la médiation publique, l’information étant accessible en ligne pour les usagers divers, mais aussi le chercheur.
Dès le début de la recherche, lorsque l’usager clique sur l’onglet Collection à partir de la page d’accueil, le site suggère quatre avenues.
- Collections Online – ensemble des collections disponibles en ligne
– Digital Outreach – traite des défis et intérêts d’intégrer le numérique dans les musées.
- Blog – nouvelles muséales et informations additionnelles sur des expositions en cours, certains artefact, etc.
– Read, Watch, Play – modèle interactif de découverte grâce à des photos, vidéos, quizzes, etc.
Chacune de ces options est accompagnée d’une brève description, permettant à la personne de sélectionner adéquatement le lien qu’elle souhaite explorer. Le mandat du catalogue en ligne semble avoir été efficacement séparé en quatre, rendant déjà l’exploration du site moins intimidante.
Quant aux collections, elles sont disponibles en version numérique sous le premier onglet ci-haut. C’est donc sur celui-ci que nous nous concentrerons.  
Le site annonce pouvoir livrer de l’information au sujet de plus de 1 million d’œuvres, d’objets, et de spécimens, et suggère ensuite des collection highlights. Ces « collection highlights » sont composées, tout comme les aperçus des artefacts qui seront suggérés lors d’une recherche spécifique, d'une photo (si disponible), de la catégorie de l’élément (objet, catégorie, publication, sujet), du titre, de l'auteur, de l'année de création, et du code d’inventaire, ce dernier reflétant explicitement le rôle interne de cette interface numérique.
La page d’accueil suggère aussi des « search tips » et « download tips », et permet aussi de choisir si l’utilisateur souhaite que tous les résultats qui seront produits par sa recherche contiennent des images, ou même des images téléchargeables.

Quels sont les critères de recherche offerts et les points d’accès proposés ?
Sur le site du Te Papa, contrairement à ce que suggèrent les articles lus en classe, la technique, la période, le mouvement artistique, etc., sont moins présents lorsque l’utilisateur initie sa recherche.
Lors d’une recherche, l’utilisateur peut utiliser les filtres qui sont à sa disposition, à savoir le type d’objet, les possibilités d’utilisation des images, et les collections auxquelles les éléments sont associés. 
Le site propose, en fait, la méthode suivante : 
– Entrer quelques mots.
– Utiliser les filtres.
– Parcourir les notices connexes.
Grâce à la page « search tips », disponible par l’entremise de la page d’accueil, le site propose aussi des alternatives et des solutions pour affiner la recherche, se mettant à la place du public en expliquant quoi faire si : « Je ne trouve pas ce que je veux, » « J’ai trop de résultats, » « Je ne trouve pas d’images, » etc.
Suggérant d’utiliser des opérateurs, des jokers, et introduisant des noms de champs de recherche courants, on voit que le musée tente de professionnaliser ses utilisateurs, et de leur donner tous les outils possibles pour bien réussir leur recherche.
Les experts et chercheurs sont aussi invités à utiliser les identifiants des objets, des intervalles de dates, de pixélisation, etc., ou même à commencer par une recherche vide pour ensuite spécifier les critères de recherche à l’aide des filtres qui se trouvent à gauche des résultats.
Pour finir, le site fait référence à Elasticsearch comme étant le système en charge de la gestion des requêtes, suggérant aux spécialistes de consulter le guide de syntaxe des chaines de requêtes de celui-ci pour toutes interrogations particulièrement complexes.
 
Quelles informations relatives aux artefacts sont-elles proposées aux utilisateurs ?
Le catalogue de Te Papa privilégie des données factuelles, mais intègre aussi quelques données iconographiques, bien que le standard descriptif reste de mise. À première vue, des initiatives telles que le « tag » d’utilisateur ne sont pas intégrées à l’interface du musée.
Les données descriptives disponibles dépendent aussi du type d’élément. Voici un tableau proposant une vue d’ensemble plutôt sommaire des informations affichées selon le type d’artefact, catégorisés par le Te Papa.

Objet: Titre / Nom
Type
Collection à laquelle l’objet appartient
Image(s)
Provenance
Statut des droits d’auteurs
Production
Classification
Matériel
Dimensions
Numéro d’inventaire
« Overview »
Références bibliographiques de « l’overview »
 
Spécimen: Nom scientifique
Statut du type
Embranchement
Classe
Ordre
Famille
Genre
Collecté par
Lieu de collecte
Identifié par
Numéro d’enregistrement
Provenance

Un élément que j’ai trouvé particulièrement intéressant est que, lorsque l’information n’est pas disponible, le Te Papa ne note pas N/A ou quelque autre convention du même type, ils omettent simplement d’écrire quoi que ce soit, de sorte que l’utilisateur qui ne consulte qu’un ou deux artefacts pourrait ne pas savoir qu’il manque une information, s’il tente de faire un recensement complet des informations sur l’objet en question. Je trouve cela dommage, ça enlève l’opportunité aux gens de creuser plus loin comme ils ne savent pas qu’il reste quelque chose à aller chercher qui pourrait être disponible, ou qui devrait l’être dans les conditions idéales.
 
Quels sont les rebonds et les liens proposés entre les artefacts ?
Les catalogueurs ont également créé des liens entre les notices, qu’ils encouragent le public à explorer. De ces méthodes, on recense des hiérarchies arborescentes, du contenu connexe que l’on peut ensuite filtrer (« tous », « se rapporte à », « destiné à », « à propos de »), des suggestions d’approfondissement concernant la recherche effectuée qui offrent des liens vers du contenu connexe, ainsi que des pages pertinentes sur le Web.
Les échos iconographiques se font également sentir comme les catégories « depicts » et « about », qui pourraient suggérer d’autres artefacts affichant des explorateurs et concernant la découverte par exemple, sont aussi présentes au sein de l’interface de Te Papa.
Il est aussi possible d’accéder à des cartes interactives suggérant des « associated places », ou l’endroit où un spécimen fut extrait, et de trouver dans la section « explorer plus d’informations » des liens vers des ensembles unis par leur matériel, le type d’artefact, le rôle escompté de l’objet, et les influences marquantes à sa formation (culturelles, technologiques, etc.).
Pour les spécimens, la taxonomie complète étant accessible, il est aussi possible de cliquer sur des sous-catégories telles qu’animal, arthropode, opilions, etc., et d’accéder aux autres spécimens correspondant à ces critères.
Pour finir, l’interface du musée propose aussi un filtre « collaboration », qui permet d’accéder aux artefacts qui découlent directement d’un effort conjoint tel que l’album de Wiki Baker et de la chorale maorie de Nouvelle-Zélande, par exemple.

Comment les contenus sont-ils éditorialisés, quels enrichissements sont proposés ?
Le catalogue en ligne est présenté comme un objet éditorial qui prolonge la tradition des catalogues imprimés et des « musées de papier », et construit donc clairement, grâce à ces nombreux liens, des récits sur la collection, tout en permettant un tri, filtre et interaction efficace.
L’interface de Te Papa, qui fait ceci à merveille, reste tout de même peu complexe. Lorsque l’utilisateur effectue une recherche, un ensemble d’artefacts s’affiche, au travers desquels le chercheur doit ensuite défiler.
Cependant, lorsque l’on clique sur un objet spécifique, la métaphore du musée « physique » se fait sentir. La photo principale et les prises de vues alternatives sont mises de l’avant sur un fond plus foncé qui rappelle un mur, et les informations se trouvent en dessous, sur un fond blanc, tel un cartel qui agit comme second point de contact avec le visiteur.  
Quant aux enrichissements, le seul recensé dans les articles de la semaine qui est réellement présent au Te Papa est la valeur d’un thésaurus iconographique, et il reste quand même peu intégré. Effectivement, le social tagging est absent, mais grâce à la tentative de création de lien par la catégorie « depict », on observe l’influence d’institutions comme Tate Online au sein du Te Papa. 
 
Quel discours sur la collection semble proposer le musée avec ce catalogue en ligne ?
Avec ce catalogue en ligne, Te Papa produit le discours institutionnel suivant :
1.  Les collections devraient être facilement partagées entre les institutions et avec les usagers. L’accent placé sur la disponibilité et les méthodes de distribution des images suggère un souhait qu’elles soient facilement diffusées à l’externe, par des professionnels mais aussi par des visiteurs sans connaissances spécifiques, désir qui est principalement suggéré par le guide « How to Download ? ». a
2.  Ils souhaitent que les liens entre les artefacts et l’histoire de la Nouvelle-Zélande soient mis de l’avant de manière interactive, introduisant des cartes et une multitude d’hyperliens. De plus, l’histoire coloniale, et donc parfois changée et réécrite, de l’État et de ses communautés, doit être explorée, intention suggérée par les indicateurs tels que « intended for », « influenced by », mais aussi certaines différenciations comme « created by » et « belonged to ».
3.  Ils veulent que l’éditorialisation symbolise la visite au musée et enseigne au public comment lire, manipuler, et interpréter les œuvres d’une manière qui se traduit facilement du numérique au « en personne ».
4.  Par sa facilité de navigation, mais aussi par l’accessibilité de l’information destinée aux chercheurs, Te Papa souhaite accueillir sur son site à la fois chercheurs et visiteurs, tentant de dialoguer avec les deux à la fois.





