title: msl6517-md
description: zrenaudie UdeM

---

# Guide **Markdown**

Markdown est un **langage de balisage léger** : il transforme du texte simple en texte structuré (titres, listes, liens…). Idéal pour la recherche, la documentation, les notes, GitHub, etc.

Documentation officielle : <https://www.markdownguide.org/>

---
## Quelques bons outils pour écrire en Markdown

* **Obsidian** 
* **Typora** 
* **Zettlr** 

Plus avancés :
* **VS Code** 
* **GitHub / GitLab** 

---

## 1. Les bases indispensables

### **Titres**

Utilise `#` :

```md
# Titre 1
## Titre 2
### Titre 3
```

---

### **Texte en gras / italique**

```md
*italique*
**gras**
***gras italique***
```

---

### **Listes**

**Listes à puces :**

```md
- élément
- élément
  - sous-élément
```

**Listes numérotées :**

```md
1. Premier point
2. Deuxième point
```

---

### **Liens**

```md
[texte du lien](https://exemple.com)
```

---

### **Images**

```md
![texte alternatif](URL-de-l-image)
```

---

### **Citations**

```md
> Ceci est une citation
>> Citation imbriquée
```

---

### **Code**

**Inline :**

```md
Voici du `code`.
```

**Bloc :**

<pre>
```langage
Du code ici
```
</pre>

---

## 2. Structurer un document

Un bon document Markdown suit cette structure :

```md
# Titre du document

## Introduction
Bref contexte.

## Section principale
- Un point
- Un autre point

### Sous-section
Texte, citation, code, etc.

## Conclusion
Résumé, ouverture.
```

---

## 3. Tableaux

```md
| Colonne 1 | Colonne 2 |
|----------|-----------|
| donnée A | donnée B  |
| donnée C | donnée D  |
```

---

## 4. Notes de bas de page

Si utilisé (selon le moteur Markdown) :

```md
Voici un texte avec une note[^1].

[^1]: Ceci est la note.
```

---

## 5. Séparateur

```md
---
```

---
