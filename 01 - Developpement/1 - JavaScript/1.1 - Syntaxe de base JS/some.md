---
title: Méthode .some() en JavaScript
tags: [javascript, array, méthode, some, débutant]
created: 2025-06-09
---

# Méthode .some() en JavaScript

## 🧠 Résumé rapide

> `.some()` teste si **au moins un élément** du tableau satisfait une condition. Elle retourne `true` ou `false`.

---

## liens web

[MDN]()
[w3school]()

---

## 📌 Contenu

### 📍 Exemple simple

```js

const nombres = [1, 3, 5, 8];

const contientPair = nombres.some(n => n % 2 === 0);

  

console.log(contientPair); // true

```

### 📍 Avec objets

```js

const utilisateurs = [

  { nom: "Paul", connecté: false },

  { nom: "Anna", connecté: true }

];

  

const aDesConnectés = utilisateurs.some(u => u.connecté);

console.log(aDesConnectés); // true

```

---

## 🔗 Liens connexes

- [[some]]
- [[find]]  

---

## 🧭 Navigation / Contexte

📂 Dossier : `01 - Développement/1.1 - JavaScript`  

🔍 Vue locale : `Méthodes des tableaux`

---

## 🗒️ Notes personnelles

- Très utile pour vérifier si **au moins une condition est remplie**

- Ne modifie pas le tableau