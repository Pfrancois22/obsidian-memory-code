---
title: Méthode .filter() en JavaScript
tags: [javascript, array, méthode, filter, débutant]
created: 2025-06-09
---

# Méthode .filter() en JavaScript  

## 🧠 Résumé rapide  

> `.filter()` permet de créer un nouveau tableau contenant uniquement les éléments qui passent un test (fonction de filtre).

---

## liens web

[MDN](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Array/filter)
[w3school](https://www.w3schools.com/jsref/jsref_filter.asp)

---

## 📌 Contenu

### 📍 Exemple de base

```js

const nombres = [1, 2, 3, 4, 5];

const pairs = nombres.filter(n => n % 2 === 0);

  

console.log(pairs); // [2, 4]

```

### 📍 Avec des objets

```js

const utilisateurs = [

  { nom: "Marie", actif: true },

  { nom: "Paul", actif: false }

];

  

const actifs = utilisateurs.filter(u => u.actif);

console.log(actifs); // [{ nom: "Marie", actif: true }]

```

---

## 🔗 Liens connexes

- [[map]]
- [[reduce]]

---

## 🧭 Navigation / Contexte

📂 Dossier : `01 - Développement/1.1 - JavaScript`  

🔍 Vue locale : `Méthodes des tableaux`

  

---

  

## 🗒️ Notes personnelles

  

- `.filter()` ne modifie pas le tableau original

- On l’utilise souvent avec `.map()` enchaîné