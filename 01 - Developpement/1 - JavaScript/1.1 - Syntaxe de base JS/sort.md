---
title: Méthode .sort() en JavaScript
tags: [javascript, array, méthode, sort, débutant]
created: 2025-06-09
---

# Méthode .sort() en JavaScript

## 🧠 Résumé rapide

> `.sort()` trie les éléments d’un tableau **en place**. Elle modifie le tableau original.

---

## liens web

[MDN]()
[w3school]()

---

## 📌 Contenu

### 📍 Tri alphabétique

```js

const fruits = ["banane", "pomme", "abricot"];

fruits.sort();

console.log(fruits); // [ "abricot", "banane", "pomme" ]

```

### 📍 Tri numérique

```js

const scores = [20, 5, 100];

scores.sort((a, b) => a - b);

console.log(scores); // [5, 20, 100]

```

---

## 🔗 Liens connexes

- [[map]]
- [[filter]]

---

## 🧭 Navigation / Contexte

📂 Dossier : `01 - Développement/1.1 - JavaScript`  

🔍 Vue locale : `Méthodes des tableaux`

---

## 🗒️ Notes personnelles

- ⚠️ Modifie le tableau original !

- Penser à faire une copie avec `[...array].sort()` si besoin