---
title: Fonctions en JavaScript
tags: [javascript, function, débutant]
created: 2025-06-09
---

# Fonctions en JavaScript

## 🧠 Résumé rapide

> Les fonctions permettent de regrouper des blocs de code réutilisables.  

> JavaScript propose plusieurs façons de les écrire : déclarées, anonymes, fléchées.

---

## liens web

[MDN – Fonctions](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Functions)  
[w3schools (EN) – JavaScript Functions](https://www.w3schools.com/js/js_functions.asp)

---

## 📌 Contenu

### 📍 Fonction déclarée (nommée)

```js
function bonjour() {
  console.log("bonjour toto");
}

bonjour(); // Affiche : bonjour toto
```

---

### 📍 Fonction anonyme affectée à une variable

```js
const salut = function () {
  console.log("Salut");
};

salut(); // Affiche : Salut
```

---

### 📍 Fonction fléchée (arrow function)

```js
const hi = () => console.log("hello");
hi(); // Affiche : hello
```

📝 Les fonctions fléchées sont souvent utilisées avec les méthodes des tableaux comme `.map()`, `.filter()`...

---

### ⚠️ Attention avec le `this`

```js
const film = {
  name: "Seven",
  start: "Brad Pitt",
  printDetails() {
    console.log(`${this.name} with ${this.start}`);
  }
};

film.printDetails(); // Affiche : Seven with Brad Pitt
```

⚠️ N’utilise **pas** `this` dans une **fonction fléchée** à l'intérieur d’un objet. Elle n’a pas son propre `this`.

---

### 📍 Exemple avec filter() et fonctions

```js
const people = [

  {name: "Miguel", age: 28},
  {name: "François", age: 61},
  {name: "Jean", age: "Deceded"}
];

console.log(
  people.filter(function (person) {
    return person.age != "Deceded";
  })
);

console.log(
  people.filter((men) => men.age == "Deceded")
);
```

---

## 🔗 Liens connexes

- [[Méthode .filter() en JavaScript]]
- [[Fonction fléchée =>]]

---

## 🧭 Navigation / Contexte

📂 Dossier : `01 - Développement/1.1 - JavaScript`  

🔍 Vue locale : `Syntaxe de base JS`

---

## 🗒️ Notes personnelles

  

- Les fonctions fléchées sont pratiques mais attention à leur comportement avec `this`.