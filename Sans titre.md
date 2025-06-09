---
titre: Plugin VSC : ESLint  
tags: [développement, typescript, react, qualité-code, eslint, vsc]  
date: {{date:YYYY-MM-DD}}  
type: plugin  
---

# Plugin VSC : ESLint

## 🧠 Résumé rapide

> Le plugin ESLint pour Visual Studio Code permet de détecter et corriger en temps réel les erreurs et incohérences de code JavaScript/TypeScript (et React), grâce à un système de règles personnalisables et à son intégration avec d’autres outils (Prettier, Husky, etc.).

---

## 📌 Contenu

### 1. Installation

- Depuis VSCode : Marketplace → “ESLint” → Installer  
- Dans votre projet :  
```npm install --save-dev eslint```


### 2. Configuration de base

Créer un fichier .eslintrc.js à la racine du projet :

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

### 3. Règles courantes et utiles

- no-console : interdire les console.log en production  
  (voir : https://palantir.github.io/tslint/rules/no-console/)  
- react-hooks/rules-of-hooks : bon usage des Hooks React  
- @typescript-eslint/no-unused-vars : détecter les variables inutilisées  
- prettier/prettier : s'assurer du bon formatage du code  

### 4. Intégration TypeScript & React

Installer les dépendances nécessaires :

    npm install --save-dev @typescript-eslint/parser @typescript-eslint/eslint-plugin
    npm install --save-dev eslint-plugin-react eslint-plugin-react-hooks

Ajouter les extensions suivantes :

    ```extends: [
      'plugin:@typescript-eslint/recommended',
      'plugin:react/recommended'
    ]```

### 5. Commandes & auto-correction

- Lancer le linter :  
  ```npm run lint```

- Directement :  
  ```npx eslint . --ext .js,.jsx,.ts,.tsx```

- Corriger automatiquement :  
  ```npm run lint -- --fix```

### 6. Astuces avancées

Auto-fix à l’enregistrement (dans les paramètres de VSCode) :

    ```"editor.codeActionsOnSave": {
      "source.fixAll.eslint": true
    }```

Pré-commit avec Husky :

    ```npm install --save-dev husky lint-staged```

Ajouter dans package.json :

    ```"husky": {
      "hooks": {
        "pre-commit": "lint-staged"
      }
    },
    "lint-staged": {
      "*.{js,ts,jsx,tsx}": ["eslint --fix", "git add"]
    }```

---

## 🔗 Liens connexes

- ESLint Guide : https://eslint.org/docs/user-guide/getting-started  
- TypeScript ESLint : https://typescript-eslint.io/  
- Extension VSCode ESLint : https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint  
- TSLint no-console : https://palantir.github.io/tslint/rules/no-console/  
- [[Autres plugins VSCode]]

---

## 🧭 Navigation / Contexte

📂 Dossier : 01 - Développement/1.2 - React  
🔍 Vue locale : React + TypeScript + Linter

---

## 🗒️ Notes personnelles

- Tester `--fix-dry-run` avant validation automatique  
- Adapter les règles pour la production  
- Créer une fiche “Husky & Lint-Staged” à part  
- Documenter les règles personnalisées dans le README

---