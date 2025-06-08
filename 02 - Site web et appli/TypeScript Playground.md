---
titre: Typescript Playground
tags: [typescript, outil, débutant, obsidian]
related: [Transcompiler TypeScript avec VSC]
---


# 📘 [TypeScript Playground](https://www.typescriptlang.org)

C'est un **site officiel** qui te permet de **transcrire ton code TypeScript** en JavaScript (et de voir le résultat en direct).

> 🧠 *Transcrire* ici, ça veut dire convertir ton code TypeScript en un code JavaScript compréhensible par ton navigateur ou Node.js.

---

## ⚙️ Configuration avant de coder

Avant d’écrire du code, on peut **choisir ses réglages** :

- **Lang** : la langue dans laquelle tu codes.
  - Exemple : TypeScript (c’est notre choix ici).
- **Target** : la version JavaScript que tu veux obtenir.
  - Exemple : `ES5`, `ES6`, etc.  
  - Plus le chiffre est haut, plus la version est récente.
- **JSX** : pour dire si tu utilises React.
  - Exemple : choisis `React` si tu codes un composant React.
- **Module** : le type de module pour l’exécution.
  - Exemple :
    - `Node` pour un code exécuté côté serveur (avec Node.js),
    - `Browser` pour un code côté navigateur,
    - `VSC` si tu utilises Visual Studio Code.

---

## 🛠️ Utiliser le Playground

Une fois ta config choisie, clique sur `Playground`.

- 🧩 **À gauche** : ton code TypeScript.
- 🧩 **À droite** : le code JavaScript généré automatiquement.

Tu peux tester ton code et voir **en direct ce que ça donne une fois transformé**.

---

## 🔍 Petit exemple

```ts
// Code TypeScript à gauche
function sayHello(name: string): string {
  return "Bonjour " + name;
}


// Résultat JavaScript à droite (selon les réglages choisis)
function sayHello(name) {
    return "Bonjour " + name;
}```

## ✅ Pourquoi c'est utile ?

- Pour **comprendre comment TypeScript devient JavaScript**.
    
- Pour **tester ton code rapidement** sans rien installer.
    
- Pour **voir les erreurs ou les avertissements** directement.

---

## 🔗 Liens connexes

### 📚 Concepts liés
- [[Typescript Playground]]
- [[]]

### 🛠️ Fiches pratiques
- [[]]
- [[]]

### 🚧 En cours
- [[]]