---
title: Événements (event) en JavaScript
tags: [javascript, event, dom, débutant]
created: 2025-06-09
---

# Événements (event) en JavaScript

## 🧠 Résumé rapide

> Un **événement** est une action utilisateur ou système (clic, touche, chargement...) capturable par JavaScript.

---

## liens web

[MDN – Introduction aux événements](https://developer.mozilla.org/fr/docs/Learn/JavaScript/Building_blocks/Events)  
[w3schools (EN)](https://www.w3schools.com/js/js_events.asp)

---

## 📌 Contenu

### 📍 Exemple simple

```js
function direBonjour() {

  alert("Bonjour !");

}  

document.querySelector("button").addEventListener("click", direBonjour);
```

---

## 🔗 Liens connexes

- [[listener]]

  

---

  

## 🧭 Navigation / Contexte

  

📂 Dossier : `01 - Développement/1.1 - JavaScript`  

🔍 Vue locale : `DOM et interactions`

  

---

  

## 🗒️ Notes personnelles

  

- L’événement courant est passé automatiquement à la fonction callback.