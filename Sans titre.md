---
title: async / await en JavaScript
tags: [javascript, async, await, promise, débutant]
created: 2025-06-09
---  

# async / await en JavaScript

## 🧠 Résumé rapide

> `async` et `await` permettent d’écrire du code asynchrone de manière **plus lisible**, comme du code synchrone.

---

## liens web

[MDN – async function](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Statements/async_function)  
[w3schools (EN)](https://www.w3schools.com/js/js_async.asp)

---

## 📌 Contenu

### 📍 Exemple

```js
function attendre(ms) {
  return new Promise(resolve => setTimeout(resolve, ms));
}  

async function saluer() {

  console.log("Bonjour");

  await attendre(2000);

  console.log("Après 2 secondes");

}
saluer();
```

---

## 🔗 Liens connexes

- [[promise]]

---

  

## 🧭 Navigation / Contexte

  

📂 Dossier : `01 - Développement/1.1 - JavaScript`  

🔍 Vue locale : `Asynchrone`

  

---

  

## 🗒️ Notes personnelles

  

- Très utilisé pour les appels API (ex: `fetch`)