---
titre: Plugin VSC : ESLint
tags: [développement, typescript, react, qualité-code, eslint, vsc]
date: {{date:2025-06-09}}
type: plugin
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
npm install --save-dev eslint```


### 2. Configuration de base

Créez un fichier `.eslintrc.js` à la racine :

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
    // Exemple : autoriser les exports constants pour React Refresh
    'react-refresh/only-export-components': [
      'warn',
      { allowConstantExport: true }
    ],
    // Ajouter ou surcharger d’autres règles ici…
  }
};
```