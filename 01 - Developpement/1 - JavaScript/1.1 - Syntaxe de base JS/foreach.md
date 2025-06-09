---
title: Méthode .forEach() en JavaScript
tags: [javascript, foreach, tableau, débutant]
created: 2025-06-09
---

# Méthode .forEach() en JavaScript

## 🧠 Résumé rapide

> `.forEach()` exécute une fonction sur chaque élément du tableau. Elle ne retourne rien.

---

## liens web

[MDN](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach)  
[w3schools](https://www.w3schools.com/jsref/jsref_foreach.asp)

---

## 📌 Contenu

### 📍 Exemple

```js

const fruits = ["🍎", "🍌", "🍊"];

  

fruits.forEach((fruit, index) => {

  console.log(index + ": " + fruit);

});

```

---

## 🔗 Liens connexes

- [[for-loop]]
- [[map]]

---

## 🧭 Navigation / Contexte

📂 Dossier : `01 - Développement/1.1 - JavaScript`  

🔍 Vue locale : `Syntaxe de base JS`

---

## 🗒️ Notes personnelles

- Ne retourne pas de valeur → pas de chaînage