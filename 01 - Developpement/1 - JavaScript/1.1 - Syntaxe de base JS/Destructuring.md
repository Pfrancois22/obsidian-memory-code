---
title: Déstructuration (Destructuring) en JavaScript
tags: [javascript, destructuring, tableau, objet, débutant]
created: 2025-06-09
---

# Déstructuration (Destructuring) en JavaScript

## 🧠 Résumé rapide

> La déstructuration permet d'extraire facilement des valeurs depuis des tableaux ou objets, en les assignant à des variables.

---
## liens web

---

## 📌 Contenu

### 📍 Avec des objets

```js

const personne = { nom: "Luc", age: 40 };

const { nom, age } = personne;

  

console.log(nom); // Luc

console.log(age); // 40

```

### 📍 Avec des tableaux

```js

const notes = [14, 18, 20];

const [maths, anglais, info] = notes;

  

console.log(anglais); // 18

```

### 📍 Valeurs par défaut

```js

const { pays = "France" } = {};

console.log(pays); // France

```

---

## 🔗 Liens connexes

- [[Operateur Rest(...)]]
- [[Operateur Spread(...)]]

---

## 🧭 Navigation / Contexte

📂 Dossier : `01 - Développement/1.1 - JavaScript`  

🔍 Vue locale : `Syntaxe de base JS`

---

## 🗒️ Notes personnelles

- Très pratique avec les props en React