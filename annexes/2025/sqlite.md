title: MSL6517-13
description: zoerenaudie UdeM
theme: presentation/theme/remark-dark.css
name: inverse
layout: true
class: inverse

---
layout: false 
# SQL

???
SQL sert à parler avec une base de données relationnelle.

créer des tables

ajouter / modifier / supprimer des données

interroger les données

définir des relations et des règles

Pas seul language mais le plus commun. 

@todo : faire cette base pour la collection du cours

---
| Critère                 | **SQLite**          | **MySQL**        | **PostgreSQL**               |
| ----------------------- | ------------------- | ---------------- | ---------------------------- |
| Type                    | Base **embarquée**  | Serveur DB       | Serveur DB                   |
| Installation            | Aucune (un fichier) | Oui              | Oui                          |
| Utilisateurs simultanés | 1–quelques          | Plusieurs        | Plusieurs                    |
| Transactions            | Oui                 | Oui              | Oui (très robuste)           |
| Contraintes             | Limitées            | Bonnes           | Très avancées                |
| Extensibilité           | Faible              | Moyenne          | Très forte                   |
| Usage typique           | Prototypage, local  | Applications web | Recherche, données complexes |


---
# SQLITE 
## Pré-requis
### en ligne 
https://sqliteonline.com/
https://beta.sqliteviewer.app/Northwind_small.sqlite/table/Category

---
### avec logiciel opensource libre et gratuit
avec visualisation : https://sqlitebrowser.org/
VS Code + extension SQLite 

---
### en local (terminal) 
**SQLite en ligne de commande**, sur ton propre ordinateur.

#### Installer SQLite (si ce n’est pas déjà fait)

##### macOS ou Linux

SQLite est **déjà installé** dans la plupart des cas.
Vérifie avec :

```bash
sqlite3 --version
```

Si tu vois un numéro de version (ex : `3.45.0`), c’est bon.

##### Windows

1. Va sur [https://www.sqlite.org/download.html](https://www.sqlite.org/download.html)
2. Télécharge **sqlite-tools** (fichier ZIP)
3. Décompresse-le dans un dossier, par exemple :
   `C:\sqlite\`
4. Ouvre l’invite de commande (`cmd`)
   et tape :

   ```bash
   cd C:\sqlite
   sqlite3
   ```

   (Tu peux aussi double-cliquer sur `sqlite3.exe`)

---

#### Créer une base de données

Dans le terminal, choisis où tu veux travailler (par exemple ton dossier Documents) :

```bash
cd ~/Documents
```

Puis crée ta base :

```bash
sqlite3 expositions.db
```

SQLite va s’ouvrir et tu verras une invite comme :

```
SQLite version 3.45.0
Enter ".help" for usage hints.
sqlite>
```


---

#### Créer tes tables et le reste

Copie-colle les commandes (ou tape-les) directement dans ton terminal. 

#### Sauvegarder et quitter

Ta base `expositions.db` est automatiquement sauvegardée à chaque changement.

Pour quitter :

```sql
.exit
```

--

##  Étape 1 : Définir le but de la base

### Objectif

Documenter des **expositions**, avec :

* les **artistes** participants,
* les **œuvres** présentées,
* et les **expositions** elles-mêmes.

---

##  Étape 2 : Concevoir le modèle

### Les tables nécessaires

| Table             | Description                               | Exemple de colonnes                             |
| ----------------- | ----------------------------------------- | ----------------------------------------------- |
| **Artiste**       | Informations sur les artistes             | `id`, `nom`, `pays`, `date_naissance`           |
| **Oeuvre**        | Informations sur les œuvres               | `id`, `titre`, `annee`, `id_artiste`            |
| **Exposition**    | Informations sur les expositions          | `id`, `titre`, `lieu`, `date_debut`, `date_fin` |
| **Participation** | Table de lien entre œuvres et expositions | `id_oeuvre`, `id_exposition`                    |

---

## Étape 3 : Créer les tables (sur [sqliteonline.com](https://sqliteonline.com))

Colle et exécute ce code :

```sql
-- Table des artistes
CREATE TABLE Provenance (
  id INTEGER PRIMARY KEY AUTOINCREMENT,
  nom TEXT NOT NULL,
  lieu TEXT
);

-- Table des œuvres
CREATE TABLE Objets (
  id INTEGER PRIMARY KEY AUTOINCREMENT,
  titre TEXT NOT NULL,
  annee INTEGER,
  id_provenance INTEGER,
  FOREIGN KEY (id_provenance) REFERENCES Provenance(id)
);


```

---

##  Étape 4 : Ajouter quelques données

```sql
INSERT INTO Provenance (titre, lieu)
VALUES ('Coll MSL', 'Canada', '1925-09-09'),
       ('Maison des Marionnettes', 'Mexique', '1907-07-06');

INSERT INTO Oeuvre (titre, annee, id_artiste)
VALUES ('Pavane', 1963, 1),
       ('La columna rota', 1944, 2)

```

---

##  Étape 5 : Interroger la base

### Voir les artistes :

```sql
SELECT * FROM Artiste;
```

### Voir les œuvres exposées avec leur artiste :

```sql
SELECT Oeuvre.titre, Artiste.nom
FROM Oeuvre
JOIN Artiste ON Oeuvre.id_artiste = Artiste.id;
```

### Voir toutes les œuvres présentées dans une exposition :

```sql
SELECT Exposition.titre AS exposition, Oeuvre.titre AS oeuvre, Artiste.nom AS artiste
FROM Participation
JOIN Oeuvre ON Participation.id_oeuvre = Oeuvre.id
JOIN Artiste ON Oeuvre.id_artiste = Artiste.id
JOIN Exposition ON Participation.id_exposition = Exposition.id;
```

---

Vues

---

## Principe général

Une vue est créée à partir d’une requête :

```sql
CREATE VIEW nom_de_la_vue AS
SELECT ... FROM ...
```

Ensuite, tu peux simplement faire :

```sql
SELECT * FROM nom_de_la_vue;
```

---

###  Vue : œuvres avec leur artiste

Cette vue combine les tables **Oeuvre** et **Artiste**.

```sql
CREATE VIEW vue_oeuvres_artistes AS
SELECT 
  Oeuvre.id AS id_oeuvre,
  Oeuvre.titre AS titre_oeuvre,
  Oeuvre.annee,
  Artiste.nom AS artiste,
  Artiste.pays
FROM Oeuvre
JOIN Artiste ON Oeuvre.id_artiste = Artiste.id;
```

 Ensuite, tu peux simplement faire :

```sql
SELECT * FROM vue_oeuvres_artistes;
```

---

###  Vue : expositions avec les œuvres et artistes

Ici, on regroupe les quatre tables pour voir *tout* d’un coup :

```sql
CREATE VIEW vue_expositions_completes AS
SELECT 
  Exposition.titre AS exposition,
  Exposition.lieu,
  Exposition.date_debut,
  Exposition.date_fin,
  Oeuvre.titre AS oeuvre,
  Artiste.nom AS artiste
FROM Participation
JOIN Oeuvre ON Participation.id_oeuvre = Oeuvre.id
JOIN Artiste ON Oeuvre.id_artiste = Artiste.id
JOIN Exposition ON Participation.id_exposition = Exposition.id;
```
 Puis tu peux interroger cette vue simplement :

```sql
SELECT * FROM vue_expositions_completes;
```

Exemple de résultat :

| exposition         | lieu                     | œuvre           | artiste            |
| ------------------ | ------------------------ | --------------- | ------------------ |
| Dialogues Modernes | Musée d’Art Contemporain | Pavane          | Jean-Paul Riopelle |
| Dialogues Modernes | Musée d’Art Contemporain | La columna rota | Frida Kahlo        |

---

###  Vue : œuvres par pays d’artiste

Une vue utile pour des statistiques rapides :

```sql
CREATE VIEW vue_oeuvres_par_pays AS
SELECT Artiste.pays, COUNT(Oeuvre.id) AS nombre_oeuvres
FROM Oeuvre
JOIN Artiste ON Oeuvre.id_artiste = Artiste.id
GROUP BY Artiste.pays;
```
 Interroger :

```sql
SELECT * FROM vue_oeuvres_par_pays;
```

Résultat :

| pays    | nombre_oeuvres |
| ------- | -------------- |
| Canada  | 1              |
| Mexique | 1              |

---

### Gérer les vues

| Action                 | Commande                                                                       |
| ---------------------- | ------------------------------------------------------------------------------ |
| Voir la liste des vues | `.tables` (dans SQLite) ou `SELECT name FROM sqlite_master WHERE type='view';` |
| Supprimer une vue      | `DROP VIEW vue_expositions_completes;`                                         |
| Modifier une vue       | `DROP VIEW ...` puis `CREATE VIEW ...` à nouveau                               |

---


Les **vues** :

* simplifient les requêtes fréquentes ;
* servent à protéger les données (tu peux cacher certaines colonnes sensibles) ;
* permettent de partager facilement une "vue" cohérente du système de données à d'autres utilisateurs ou outils.


--- 

Export


---
# MySql

---

## Pré-requis (localement)

MAMP et XAMPP pour linux -> open WebStart page -> tool -> MyPhpAdmin 

## Pré-requis (en ligne)

* **DB Fiddle (MySQL 8.x)**
  [https://dbfiddle.uk/g2u6-4AX](https://dbfiddle.uk/g2u6-4AX)

  * Colonne de gauche : **Schema SQL**
  * Colonne de droite : **Query SQL**

Dans dbfiddle :

* tout le schéma (CREATE TABLE, INSERT, VIEW) va **dans Schema SQL**
* les SELECT vont **dans Query SQL**

---

## Étape 1 : Définir le but de la base

### Objectif

Documenter :

* des **artistes**
* des **œuvres**
* des **expositions**
* leurs **relations** (œuvres exposées)

---

## Étape 2 : Concevoir le modèle

### Tables nécessaires

| Table         | Rôle                                |
| ------------- | ----------------------------------- |
| Artiste       | Informations biographiques          |
| Oeuvre        | Œuvres produites                    |
| Exposition    | Événements                          |
| Participation | Table de liaison œuvre ↔ exposition |

relation **n–n** entre œuvres et expositions

---

## Étape 3 : Créer les tables (MySQL)

**À coller dans *Schema SQL***

```sql
CREATE TABLE Artiste (
  id INT AUTO_INCREMENT PRIMARY KEY,
  nom VARCHAR(255) NOT NULL,
  pays VARCHAR(100),
  date_naissance DATE
);

CREATE TABLE Oeuvre (
  id INT AUTO_INCREMENT PRIMARY KEY,
  titre VARCHAR(255) NOT NULL,
  annee INT,
  id_artiste INT,
  CONSTRAINT fk_oeuvre_artiste
    FOREIGN KEY (id_artiste)
    REFERENCES Artiste(id)
);

CREATE TABLE Exposition (
  id INT AUTO_INCREMENT PRIMARY KEY,
  titre VARCHAR(255) NOT NULL,
  lieu VARCHAR(255),
  date_debut DATE,
  date_fin DATE
);

CREATE TABLE Participation (
  id_oeuvre INT,
  id_exposition INT,
  PRIMARY KEY (id_oeuvre, id_exposition),
  CONSTRAINT fk_participation_oeuvre
    FOREIGN KEY (id_oeuvre)
    REFERENCES Oeuvre(id),
  CONSTRAINT fk_participation_exposition
    FOREIGN KEY (id_exposition)
    REFERENCES Exposition(id)
);
```

### Différences clés avec SQLite

* `INTEGER PRIMARY KEY AUTOINCREMENT` → `INT AUTO_INCREMENT`
* `TEXT` → `VARCHAR`
* `DATE` est un vrai type (pas une chaîne)
* clé primaire **composite** pour la table de liaison

---

## Étape 4 : Ajouter des données

**Toujours dans Schema SQL**

```sql
INSERT INTO Artiste (nom, pays, date_naissance)
VALUES
  ('Jean-Paul Riopelle', 'Canada', '1923-10-07'),
  ('Frida Kahlo', 'Mexique', '1907-07-06');

INSERT INTO Oeuvre (titre, annee, id_artiste)
VALUES
  ('Pavane', 1963, 1),
  ('La columna rota', 1944, 2);

INSERT INTO Exposition (titre, lieu, date_debut, date_fin)
VALUES
  ('Dialogues Modernes', 'Musée d’Art Contemporain', '2024-06-01', '2024-09-30');

INSERT INTO Participation (id_oeuvre, id_exposition)
VALUES
  (1, 1),
  (2, 1);
```

---

## Étape 5 : Interroger la base

**À mettre dans Query SQL**

### Voir les artistes

```sql
SELECT * FROM Artiste;
```

---

### Œuvres avec leur artiste

```sql
SELECT
  Oeuvre.titre,
  Artiste.nom
FROM Oeuvre
JOIN Artiste ON Oeuvre.id_artiste = Artiste.id;
```

---

### Œuvres exposées dans chaque exposition

```sql
SELECT
  Exposition.titre AS exposition,
  Oeuvre.titre AS oeuvre,
  Artiste.nom AS artiste
FROM Participation
JOIN Oeuvre ON Participation.id_oeuvre = Oeuvre.id
JOIN Artiste ON Oeuvre.id_artiste = Artiste.id
JOIN Exposition ON Participation.id_exposition = Exposition.id;
```

---

# Les vues (MySQL)

## Principe général

```sql
CREATE VIEW nom_vue AS
SELECT ...
```

Puis :

```sql
SELECT * FROM nom_vue;
```

---

## Vue 1 : œuvres + artistes

**Schema SQL**

```sql
CREATE VIEW vue_oeuvres_artistes AS
SELECT
  Oeuvre.id AS id_oeuvre,
  Oeuvre.titre AS titre_oeuvre,
  Oeuvre.annee,
  Artiste.nom AS artiste,
  Artiste.pays
FROM Oeuvre
JOIN Artiste ON Oeuvre.id_artiste = Artiste.id;
```

**Query SQL**

```sql
SELECT * FROM vue_oeuvres_artistes;
```

---

## Vue 2 : expositions complètes

```sql
CREATE VIEW vue_expositions_completes AS
SELECT
  Exposition.titre AS exposition,
  Exposition.lieu,
  Exposition.date_debut,
  Exposition.date_fin,
  Oeuvre.titre AS oeuvre,
  Artiste.nom AS artiste
FROM Participation
JOIN Oeuvre ON Participation.id_oeuvre = Oeuvre.id
JOIN Artiste ON Oeuvre.id_artiste = Artiste.id
JOIN Exposition ON Participation.id_exposition = Exposition.id;
```

```sql
SELECT * FROM vue_expositions_completes;
```

---

## Vue 3 : œuvres par pays d’artiste

```sql
CREATE VIEW vue_oeuvres_par_pays AS
SELECT
  Artiste.pays,
  COUNT(Oeuvre.id) AS nombre_oeuvres
FROM Oeuvre
JOIN Artiste ON Oeuvre.id_artiste = Artiste.id
GROUP BY Artiste.pays;
```

```sql
SELECT * FROM vue_oeuvres_par_pays;
```

---

## Gérer les vues (MySQL)

| Action            | Commande                                      |
| ----------------- | --------------------------------------------- |
| Lister les vues   | `SHOW FULL TABLES WHERE TABLE_TYPE = 'VIEW';` |
| Supprimer une vue | `DROP VIEW vue_expositions_completes;`        |
| Modifier une vue  | `DROP VIEW` puis `CREATE VIEW`                |

---

# 🚀 Guide d'Installation - Application de Gestion de Contacts

## 📋 Prérequis

- **Node.js** (version 14 ou supérieure) - [Télécharger](https://nodejs.org/)
- **MySQL** (version 5.7 ou supérieure) - [Télécharger](https://dev.mysql.com/downloads/)
- Un éditeur de code (VS Code recommandé)

---

## 📦 Étape 1 : Installation de MySQL

### Sur Windows
1. Téléchargez MySQL Installer depuis le site officiel
2. Exécutez l'installateur et choisissez "Developer Default"
3. Configurez le mot de passe root
4. Démarrez le service MySQL

### Sur macOS
```bash
brew install mysql
brew services start mysql
mysql_secure_installation
```

### Sur Linux (Ubuntu/Debian)
```bash
sudo apt update
sudo apt install mysql-server
sudo mysql_secure_installation
```

---

## 🗄️ Étape 2 : Création de la base de données

1. **Connectez-vous à MySQL :**
```bash
mysql -u root -p
```

2. **Exécutez le script SQL :**
- Copiez le contenu du fichier `database.sql`
- Collez-le dans le terminal MySQL ou
- Exécutez : `source /chemin/vers/database.sql`

3. **Vérifiez la création :**
```sql
SHOW DATABASES;
USE gestion_contacts;
SHOW TABLES;
SELECT * FROM contacts;
```

---

## 🔧 Étape 3 : Installation du Backend

1. **Créez un dossier pour le projet :**
```bash
mkdir backend-contacts
cd backend-contacts
```

2. **Créez les fichiers :**
- Créez `package.json` avec le contenu fourni
- Créez `server.js` avec le code du backend

3. **Installez les dépendances :**
```bash
npm install
```

4. **Configurez la connexion MySQL dans `server.js` :**
```javascript
const db = mysql.createConnection({
  host: 'localhost',
  user: 'root',              // Votre nom d'utilisateur MySQL
  password: 'votre_mot_de_passe',  // Votre mot de passe MySQL
  database: 'gestion_contacts'
});
```

5. **Démarrez le serveur :**
```bash
npm start
```

Vous devriez voir :
```
✅ Connecté à MySQL
🚀 Serveur démarré sur le port 3001
📡 API disponible sur http://localhost:3001/api/contacts
```

---

## 🎨 Étape 4 : Configuration du Frontend React

1. **Modifiez le composant React pour utiliser l'API :**

Remplacez la section de chargement des données dans le composant React par :

```javascript
// Au début du composant, ajoutez :
const API_URL = 'http://localhost:3001/api/contacts';

// Remplacez useEffect par :
useEffect(() => {
  fetchContacts();
}, []);

const fetchContacts = async () => {
  try {
    const response = await fetch(API_URL);
    const data = await response.json();
    setContacts(data);
  } catch (error) {
    console.error('Erreur lors du chargement:', error);
  }
};

// Modifiez handleSubmit :
const handleSubmit = async () => {
  if (!formData.nom || !formData.prenom || !formData.email) {
    alert('Veuillez remplir les champs obligatoires');
    return;
  }
  
  try {
    if (editingId) {
      // Mise à jour
      await fetch(`${API_URL}/${editingId}`, {
        method: 'PUT',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify(formData)
      });
    } else {
      // Création
      await fetch(API_URL, {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify(formData)
      });
    }
    
    await fetchContacts();
    setIsAdding(false);
    setEditingId(null);
    resetForm();
  } catch (error) {
    console.error('Erreur:', error);
    alert('Erreur lors de l\'enregistrement');
  }
};

// Modifiez handleDelete :
const handleDelete = async (id) => {
  if (confirm('Êtes-vous sûr de vouloir supprimer ce contact ?')) {
    try {
      await fetch(`${API_URL}/${id}`, {
        method: 'DELETE'
      });
      await fetchContacts();
    } catch (error) {
      console.error('Erreur:', error);
      alert('Erreur lors de la suppression');
    }
  }
};
```

---

## 🧪 Étape 5 : Tests

### Tester l'API avec curl ou Postman

**1. Récupérer tous les contacts :**
```bash
curl http://localhost:3001/api/contacts
```

**2. Créer un contact :**
```bash
curl -X POST http://localhost:3001/api/contacts \
  -H "Content-Type: application/json" \
  -d '{
    "nom": "Test",
    "prenom": "Utilisateur",
    "email": "test@example.com",
    "telephone": "514-555-0000",
    "entreprise": "Test Corp",
    "poste": "Testeur"
  }'
```

**3. Mettre à jour un contact :**
```bash
curl -X PUT http://localhost:3001/api/contacts/1 \
  -H "Content-Type: application/json" \
  -d '{
    "nom": "Dubois",
    "prenom": "Marie",
    "email": "marie.dubois@example.com",
    "telephone": "514-555-9999",
    "entreprise": "Tech Corp",
    "poste": "Senior Developer"
  }'
```

**4. Supprimer un contact :**
```bash
curl -X DELETE http://localhost:3001/api/contacts/1
```

**5. Rechercher des contacts :**
```bash
curl http://localhost:3001/api/contacts/search?q=martin
```

---

## 🔍 Résolution de problèmes

### Erreur de connexion MySQL
```
Error: connect ECONNREFUSED 127.0.0.1:3306
```
**Solution :** Vérifiez que MySQL est démarré
```bash
# Windows
services.msc (chercher MySQL)

# macOS
brew services list

# Linux
sudo systemctl status mysql
```

### Erreur CORS
```
Access to fetch has been blocked by CORS policy
```
**Solution :** Vérifiez que `app.use(cors())` est bien présent dans server.js

### Port déjà utilisé
```
Error: listen EADDRINUSE: address already in use :::3001
```
**Solution :** Changez le port ou arrêtez le processus existant
```bash
# Trouver le processus
lsof -i :3001

# Tuer le processus
kill -9 <PID>
```

---

## 📚 Structure finale du projet

```
projet/
├── backend/
│   ├── server.js
│   ├── package.json
│   └── database.sql
│
└── frontend/
    └── (votre application React)
```

---

## 🎯 Prochaines étapes

- ✅ Ajouter l'authentification (JWT)
- ✅ Implémenter la pagination
- ✅ Ajouter des filtres avancés
- ✅ Créer des exports CSV/Excel
- ✅ Ajouter des validations côté serveur
- ✅ Mettre en place des logs
- ✅ Déployer en production

---

## 📞 Support

Pour toute question, vérifiez :
1. Les logs du serveur dans le terminal
2. La console du navigateur (F12)
3. Les erreurs MySQL dans les logs

Bon développement ! 🚀