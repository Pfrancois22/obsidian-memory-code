---
title: Callbacks en JavaScript
tags: [javascript, callback, fonction, débutant]
created: 2025-06-09
---

# Callbacks en JavaScript

## 🧠 Résumé rapide

> Un **callback** est une fonction passée en argument à une autre fonction,  

> qui sera exécutée **plus tard**, soit immédiatement, soit à un moment déclenché (retour).

---

## liens web

[MDN – Fonctions callback](https://developer.mozilla.org/fr/docs/Glossary/Callback_function)  
[w3schools (EN) – Callback Function](https://www.w3schools.com/js/js_callback.asp)

---

## 📌 Contenu

### 📍 Exemple de base

```js
function saluer(nom) {
  console.log("Bonjour " + nom);
}  

function traiterUtilisateur(callback) {
  const nom = "François";
  callback(nom);
}

traiterUtilisateur(saluer);
```

  
👉 Ici, `saluer` est passé **en tant que callback** à `traiterUtilisateur`.

---

### 📍 Callback anonyme

```js
setTimeout(function () {
  console.log("3 secondes se sont écoulées");
}, 3000);
```

➡️ `setTimeout` exécute la fonction **après 3 secondes**.

---

### 📍 Callback fléché

```js
const nombres = [1, 2, 3];
nombres.forEach((n) => console.log(n * 2));
```

➡️ `.forEach()` prend une fonction en paramètre → c’est un callback.

---

## 🔗 Liens connexes

- [[function]]
- [[foreach]]
 
---

## 🧭 Navigation / Contexte

📂 Dossier : `01 - Développement/1.1 - JavaScript`  

🔍 Vue locale : `Fonctions et logique`

---

## 🗒️ Notes personnelles

- Très courant avec les événements (`addEventListener`, etc.)

- Les callbacks peuvent devenir difficiles à suivre : préférer parfois `Promise` ou `async/await`