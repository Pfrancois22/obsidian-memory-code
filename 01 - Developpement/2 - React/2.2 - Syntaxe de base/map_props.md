---
title: Utiliser .map() dans les props React
tags: [javascript, react, map, props, débutant]
created: 2025-06-09
---

# Utiliser .map() dans les props React

## 🧠 Résumé rapide

> `.map()` est souvent utilisé dans React pour afficher une liste d’éléments dynamiquement dans le JSX.

---

## liens web

[React Docs - Lists and Keys](https://react.dev/learn/rendering-lists)  
[w3schools](https://www.w3schools.com/react/react_es6_map.asp)
 
---

## 📌 Contenu

### 📍 Exemple

```js

const fruits = ["🍎", "🍌", "🍊"];

export default function ListeFruits() {

  return (

    <ul>

      {fruits.map((fruit, index) => (

        <li key={index}>{fruit}</li>

      ))}

    </ul>

  );

}

```

---

## 🔗 Liens connexes

- [[Méthode .map() en JavaScript]]
- [[foreach]]
---

## 🧭 Navigation / Contexte

📂 Dossier : `02 - React/2.2 - Syntaxe de base`  

🔍 Vue locale : `JSX et rendu dynamique`

---

## 🗒️ Notes personnelles

- Ne jamais oublier la `key` quand on mappe un tableau