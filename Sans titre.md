---
title: Méthode .find() en JavaScript
tags: [javascript, array, méthode, find, débutant]
created: 2025-06-09
---

# Méthode .find() en JavaScript

## 🧠 Résumé rapide

> `.find()` retourne le **premier élément** d’un tableau qui satisfait une condition. Si rien n’est trouvé, elle retourne `undefined`.

---

## 📌 Contenu

### 📍 Exemple simple

```js

const nombres = [3, 7, 10, 15];

const premierGrand = nombres.find(n => n > 9);

  

console.log(premierGrand); // 10

```

### 📍 Avec objets

```js

const utilisateurs = [

  { nom: "Luc", admin: false },

  { nom: "Marie", admin: true }

];

  

const admin = utilisateurs.find(u => u.admin);

console.log(admin.nom); // "Marie"

```

---

## 🔗 Liens connexes

- [[includes() en JavaScript]]

- [[Méthode .some() en JavaScript]]

  

---

  

## 🧭 Navigation / Contexte

  

📂 Dossier : `01 - Développement/1.1 - JavaScript`  

🔍 Vue locale : `Méthodes des tableaux`

  

---

  

## 🗒️ Notes personnelles

  

- `.find()` renvoie l’élément, pas son index

- Utile pour vérifier la présence d’un objet ou valeur