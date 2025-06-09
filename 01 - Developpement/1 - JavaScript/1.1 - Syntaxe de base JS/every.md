---
title: Méthode .every() en JavaScript
tags: [javascript, array, méthode, every, débutant]
created: 2025-06-09
---

# Méthode .every() en JavaScript  

## 🧠 Résumé rapide  

> `.every()` teste si **tous les éléments** d’un tableau remplissent une condition. Elle retourne `true` ou `false`.

---

## 📌 Contenu

### 📍 Exemple simple

```js

const nombres = [2, 4, 6];

const tousPairs = nombres.every(n => n % 2 === 0);

console.log(tousPairs); // true

```

### 📍 Exemple avec objets

```js

const utilisateurs = [

  { nom: "Alice", actif: true },

  { nom: "Bob", actif: true }

];

  

const tousActifs = utilisateurs.every(u => u.actif);

console.log(tousActifs); // true

```

---

## 🔗 Liens connexes

- [[some]]
- [[filter]]

---

## 🧭 Navigation / Contexte

📂 Dossier : `01 - Développement/1.1 - JavaScript`  

🔍 Vue locale : `Méthodes des tableaux`

---

## 🗒️ Notes personnelles

- À l'inverse de `.some()`, vérifie si **tout est conforme**
- Ne modifie pas le tableau