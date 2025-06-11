---
title: Valeurs truthy et falsy en JavaScript
tags: [javascript, logique, conditions, débutant]
created: 2025-06-09
---  

# Valeurs truthy et falsy en JavaScript

## 🧠 Résumé rapide
  
> En JavaScript, toute valeur est automatiquement convertie en **booléen** dans un contexte logique (`if`, `while`, etc.).  

> On parle alors de valeur **truthy** (considérée comme vraie) ou **falsy** (considérée comme fausse).

---

## liens web

[MDN – Truthy](https://developer.mozilla.org/fr/docs/Glossary/Truthy)  
[MDN – Falsy](https://developer.mozilla.org/fr/docs/Glossary/Falsy)  
[w3schools (EN)](https://www.w3schools.com/js/js_booleans.asp)

---

## 📌 Contenu

### 📍 Valeurs falsy

Sont considérées comme `false` dans un test conditionnel :

```js
false

0

-0

0n         // BigInt zéro

""         // chaîne vide

null

undefined

NaN
```

Exemple :

```js
if (0) {

  console.log("ne s'affiche pas");

}

```

---

### 📍 Valeurs truthy

Tout ce qui **n’est pas falsy** est `truthy` :

```js
true

"texte"

[]           // tableau vide

{}           // objet vide

42

"0"

"false"

Infinity

-1

```

Exemple :

```js
if ("bonjour") {

  console.log("affiché");

}
```
  
---

## 🔗 Liens connexes

- [[function]]
- [[conditions]]

---

## 🧭 Navigation / Contexte

📂 Dossier : `01 - Développement/1.1 - JavaScript`  

🔍 Vue locale : `Logique et conditions`

---

## 🗒️ Notes personnelles

- Très utile pour écrire des conditions rapides : `if (valeur) { ... }`

- Bien connaître ces cas évite des bugs subtils