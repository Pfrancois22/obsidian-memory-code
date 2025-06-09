---
title: Plugin VSC ESLint
tags: [développement]

---
  
# Plugin VSC : ESLint

## 🧠 Résumé rapide

  
> Le plugin ESLint pour Visual Studio Code permet de détecter et corriger en temps réel les erreurs et incohérences de code JavaScript/TypeScript (et React), grâce à un système de règles personnalisables et à son intégration avec d’autres outils (Prettier, Husky, etc.).

  
---

## 📌 Contenu

  

### 1. Installation

  

```bash

# Depuis VSCode : Marketplace → “ESLint” → Installer

# Dans votre projet :

npm install --save-dev eslint

```

  

### 2. Configuration de base

  

Créez un fichier `.eslintrc.js` à la racine :

  

```js

module.exports = {

  parser: '@typescript-eslint/parser',

  extends: [

    'eslint:recommended',

    'plugin:@typescript-eslint/recommended',

    'plugin:react/recommended',

    'plugin:prettier/recommended'

  ],

  plugins: ['react-refresh'],

  env: {

    browser: true,

    es2021: true,

    node: true

  },

  settings: {

    react: {

      version: 'detect'

    }

  },

  rules: {

    'react-refresh/only-export-components': [

      'warn',

      { allowConstantExport: true }

    ]

  }

};

```

  

### 3. Règles courantes et utiles

  

- **no-console** : interdire les `console.log` en production  

  👉 https://palantir.github.io/tslint/rules/no-console/  

- **react-hooks/rules-of-hooks** : garantir l’utilisation correcte des Hooks React  

- **@typescript-eslint/no-unused-vars** : détecter les variables non utilisées  

- **prettier/prettier** : formater le code selon vos conventions Prettier

  

### 4. Intégration TypeScript & React

  

```bash

npm install --save-dev @typescript-eslint/parser @typescript-eslint/eslint-plugin

npm install --save-dev eslint-plugin-react eslint-plugin-react-hooks

```

  

```js

extends: [

  'plugin:@typescript-eslint/recommended',

  'plugin:react/recommended'

]

```

  

### 5. Commandes & Auto-correction

  

```bash

# Lancer le linter :

npm run lint

  

# Ou en direct :

npx eslint . --ext .js,.jsx,.ts,.tsx

  

# Corriger automatiquement :

npm run lint -- --fix

```

  

### 6. Astuces avancées

  

#### ✅ Auto-fix à l’enregistrement (VSCode)

  

```json

"editor.codeActionsOnSave": {

  "source.fixAll.eslint": true

}

```

  

#### 🪝 Hook Git avec Husky

  

```bash

npm install --save-dev husky lint-staged

```

  

Dans `package.json` :

  

```json

"husky": {

  "hooks": {

    "pre-commit": "lint-staged"

  }

},

"lint-staged": {

  "*.{js,ts,jsx,tsx}": ["eslint --fix", "git add"]

}

```

  

---

  

## 🔗 Liens connexes

  

- [ESLint • Guide officiel](https://eslint.org/docs/user-guide/getting-started)  

- [@typescript-eslint • Docs](https://typescript-eslint.io/)  

- [Extension ESLint (VSCode)](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)  

- [TSLint : règle no-console](https://palantir.github.io/tslint/rules/no-console/)  

- [[Autres plugins VSCode]]

  

---

  

## 🧭 Navigation / Contexte

  

📂 Dossier : `01 - Développement/1.2 - React`  

🔍 Vue locale : `React + TypeScript + Linter`

  

---

  

## 🗒️ Notes personnelles

  

- Tester `--fix-dry-run` en CI avant validation automatique  

- Bien adapter les règles selon environnement (dev/prod)  

- Créer fiche liée : [[Husky & Lint-Staged]] pour workflow complet  

- Ajouter section pour Prettier si utilisé en projet