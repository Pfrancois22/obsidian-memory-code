---
title: Currying en JavaScript
tags: [javascript, fonction, avancé, currying]
created: 2025-06-09
---

# Currying en JavaScript
  
## 🧠 Résumé rapide
  

> Le **currying** est une technique qui consiste à transformer une fonction à plusieurs arguments en une **succession de fonctions** prenant un seul argument chacune.  

> Cela permet de réutiliser partiellement une fonction et d’enchaîner des appels.

  

---

  

## liens web

  

[MDN – Fonction curry](https://developer.mozilla.org/en-US/docs/Glossary/Currying)  

[Freecodecamp – Currying in JavaScript (EN)](https://www.freecodecamp.org/news/currying-in-javascript/)

  

---

  

## 📌 Contenu

  

### 📍 Exemple de fonction classique

  

```js

function add(a, b) {

  return a + b;

}

console.log(add(2, 3)); // 5

```

  

---

  

### 📍 Exemple de currying à deux niveaux

  

```js

function add1(a) {

  return function (b) {

    return a + b;

  };

}

  

const innerClosure = add1(40); // renvoie une fonction

console.log(innerClosure(21)); // 61

  

// ou directement :

console.log(add1(18)(10)); // 28

```

  

---

  

### 📍 Currying à trois niveaux

  

```js

function add3(a) {

  return function (b) {

    return function (c) {

      return a + b + c;

    };

  };

}

  

console.log(add3(20)(30)(50)); // 100

```

  

---

  

### 📍 Avec fonction fléchée

  

```js

const add4 = (a) => (b) => (c) => a + b + c;

console.log(add4(5)(15)(30)); // 50

```

  

---

  

## 🎯 À quoi ça sert concrètement ?

  

- **Réutilisation partielle** : on peut "précharger" un ou plusieurs arguments.

- Très utile dans des contextes comme :

  - Les bibliothèques fonctionnelles (`lodash`, `ramda`)

  - La programmation réactive ou fonctionnelle

  - La configuration dynamique de composants

  

**Exemple :**

```js

const saluer = (salutation) => (nom) => console.log(salutation + " " + nom);

  

const direBonjour = saluer("Bonjour");

direBonjour("Luc"); // Bonjour Luc

```

  

---

  

## 🔗 Liens connexes

  

- [[function]]

- [[arrow function]]

- [[closures]]

  

---

  

## 🧭 Navigation / Contexte

  

📂 Dossier : `01 - Développement/1.1 - JavaScript`  

🔍 Vue locale : `Fonctions avancées`

  

---

  

## 🗒️ Notes personnelles

  

- Le currying peut paraître abstrait au début, mais devient puissant dans des patterns avancés (React, logique fonctionnelle, hooks personnalisés…)