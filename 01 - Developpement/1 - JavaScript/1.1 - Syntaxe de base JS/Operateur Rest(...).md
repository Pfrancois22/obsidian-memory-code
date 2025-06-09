---
title: Opérateur Rest (...) en JavaScript
tags: [javascript, rest, opérateur, débutant]
created: 2025-06-09
---

# Opérateur Rest (...) en JavaScript

## 🧠 Résumé rapide

> L’opérateur `rest` (`...`) permet de collecter un nombre variable d’arguments dans une fonction ou de regrouper les propriétés restantes d’un objet ou tableau.

---

## 📌 Contenu

### 📍 Utilisation en fonction

```js

function addition(...nombres) {

  return nombres.reduce((acc, curr) => acc + curr, 0);

}

  

console.log(addition(1, 2, 3)); // 6

```

### 📍 Utilisation en décomposition d’objet

```js

const { nom, ...autresInfos } = {

  nom: "Alice",

  age: 30,

  ville: "Paris"

};

  

console.log(nom);         // "Alice"

console.log(autresInfos); // { age: 30, ville: "Paris" }

```

### 📍 Utilisation en décomposition de tableau

```js

const [premier, ...reste] = [1, 2, 3, 4];

console.log(premier); // 1

console.log(reste);   // [2, 3, 4]

```

---

## 🔗 Liens connexes

- [[Operateur Spread (...)]]

---

## 🧭 Navigation / Contexte

📂 Dossier : `01 - Développement/1.1 - JavaScript`  

🔍 Vue locale : `Syntaxe de base JS`

---

## 🗒️ Notes personnelles

- À bien distinguer de l'opérateur spread (`...`)

- Pratique avec les fonctions variadiques