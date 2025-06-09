---
title: Opérateur Spread(...) en JavaScript
tags: [javascript, spread, opérateur, débutant]
created: 2025-06-09
---

# Opérateur Spread(...) en JavaScript  

## 🧠 Résumé rapide  

> L’opérateur `spread` (`...`) permet de décomposer un tableau, un objet ou une chaîne pour les insérer ailleurs (fonction, tableau, etc.).  

---  

## liens web

[MDN]()
[w3school]()

---

## 📌 Contenu  

### 📍 Copie de tableau  

```js

const original = [1, 2, 3];

const copie = [...original];

console.log(copie); // [1, 2, 3]

```
  
### 📍 Fusion de tableaux
  
```js

const a = [1, 2];

const b = [3, 4];

const fusion = [...a, ...b];

console.log(fusion); // [1, 2, 3, 4]

```

### 📍 Ajout dans un objet

```js

const user = { nom: "Bob", age: 25 };

const clone = { ...user, ville: "Paris" };

console.log(clone); // { nom: "Bob", age: 25, ville: "Paris" }

```

---

## 🔗 Liens connexes

- [[Operateur Rest(...)]]

---

## 🧭 Navigation / Contexte

📂 Dossier : `01 - Développement/1.1 - JavaScript`  

🔍 Vue locale : `Syntaxe de base JS`

---

## 🗒️ Notes personnelles

- Spread permet de cloner, fusionner, insérer

- Souvent combiné avec Rest dans la même fonction