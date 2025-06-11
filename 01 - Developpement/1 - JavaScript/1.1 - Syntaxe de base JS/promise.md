---
title: Promise en JavaScript
tags: [javascript, promise, asynchrone, débutant]
created: 2025-06-09
---

# Promise en JavaScript

## 🧠 Résumé rapide

> Une Promise représente une **valeur qui sera disponible dans le futur**.  

> Elle permet de gérer du code **asynchrone** plus facilement qu’avec des callbacks.

---

## liens web

[MDN – Promise](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Promise)  
[w3schools (EN)](https://www.w3schools.com/js/js_promise.asp)

---

## 📌 Contenu

### 📍 Exemple basique

```js
const promesse = new Promise((resolve, reject) => {
  const succes = true;  

  if (succes) resolve("Tout va bien !");
  else reject("Erreur !");

});  

promesse.then((message) => {

  console.log(message);

}).catch((err) => {

  console.error(err);

});
```

---

## 🔗 Liens connexes

- [[async await]]
- [[callbacks]]

---

## 🧭 Navigation / Contexte

📂 Dossier : `01 - Développement/1.1 - JavaScript`  

🔍 Vue locale : `Asynchrone`

---

## 🗒️ Notes personnelles

- Permet d’enchaîner des actions plus facilement que les callbacks imbriqués