---
title: Listener en JavaScript
tags: [javascript, event listener, dom, débutant]
created: 2025-06-09
---

# Listener en JavaScript

## 🧠 Résumé rapide

> Un **listener** est un écouteur d’événement : il attend qu’un événement se produise pour exécuter une fonction.

---

## liens web

[MDN – addEventListener](https://developer.mozilla.org/fr/docs/Web/API/EventTarget/addEventListener)  
[w3schools (EN)](https://www.w3schools.com/jsref/met_element_addeventlistener.asp)

---

## 📌 Contenu

### 📍 Exemple avec clic

```js
const bouton = document.querySelector("button");  

bouton.addEventListener("click", () => {

  console.log("Le bouton a été cliqué !");

});
```

---

## 🔗 Liens connexes

- [[event]]

---

## 🧭 Navigation / Contexte
  
📂 Dossier : `01 - Développement/1.1 - JavaScript`  

🔍 Vue locale : `DOM et interactions`

---

## 🗒️ Notes personnelles
  

- addEventListener peut écouter plusieurs types d’événements : click, keydown, mouseover...