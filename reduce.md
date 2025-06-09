---
title: Méthode .reduce() en JavaScript
tags: [javascript, array, méthode, reduce, débutant]
created: 2025-06-09
---  

# Méthode .reduce() en JavaScript

## 🧠 Résumé rapide

> `.reduce()` permet d'accumuler les valeurs d’un tableau en une seule, selon une fonction de réduction. C’est utile pour faire des sommes, des moyennes, ou créer un objet à partir d’un tableau.

---

## 📌 Contenu

### 📍 Addition de nombres

```js

const nombres = [1, 2, 3, 4];

const total = nombres.reduce((acc, val) => acc + val, 0);

  

console.log(total); // 10

```

### 📍 Conversion tableau → objet

```js

const personnes = [

  { id: 1, nom: "Alice" },

  { id: 2, nom: "Bob" }

];

  

const parId = personnes.reduce((acc, personne) => {

  acc[personne.id] = personne.nom;

  return acc;

}, {});

  

console.log(parId); // { 1: "Alice", 2: "Bob" }

```

### 📍 Valeur de départ

- La **valeur initiale** (second argument) est importante.
- 
- Sans elle, `reduce` commence à l’indice 1 du tableau.

---

## 🔗 Liens connexes

- [[filter]]
- [[map]]

---

## 🧭 Navigation / Contexte

📂 Dossier : `01 - Développement/1.1 - JavaScript`  

🔍 Vue locale : `Méthodes des tableaux`

  

---

  

## 🗒️ Notes personnelles

  

- Si ça te semble compliqué, commence par `.map()` et `.filter()`  

- `.reduce()` est souvent utilisé pour transformer ou résumer des données complexes