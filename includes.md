---
title: Méthode .includes() en JavaScript
tags: [javascript, string, array, includes, débutant]
created: 2025-06-09
---

# Méthode .includes() en JavaScript

## 🧠 Résumé rapide

> `.includes()` vérifie si une **valeur existe** dans un tableau ou une chaîne. Elle renvoie `true` ou `false`.

---

## 📌 Contenu

### 📍 Avec un tableau

```js

const fruits = ["pomme", "banane", "orange"];

console.log(fruits.includes("banane")); // true

```

### 📍 Avec une chaîne

```js

const phrase = "Je suis débutant en JS";

console.log(phrase.includes("débutant")); // true

```
 
---

## 🔗 Liens connexes

- [[find]]
- [[some]]
---

## 🧭 Navigation / Contexte

📂 Dossier : `01 - Développement/1.1 - JavaScript`  

🔍 Vue locale : `Méthodes des tableaux`

---

## 🗒️ Notes personnelles

- Attention à la casse des lettres (Maj/Min)

- Ne fonctionne pas pour rechercher dans un objet directement