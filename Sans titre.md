



---
titre: Transcompiler TypeScript avec VSC
tags: [typescript, vscode, débutant, cli, transpilation]
---

# 🔧 Transcompiler du TypeScript dans Visual Studio Code (VSC)

Transcompiler veut dire **transformer** ton fichier `.ts` (TypeScript) en fichier `.js` (JavaScript) exécutable par ton navigateur ou Node.js.

---

## 🛠️ Étapes simples

1. **Créer un fichier TypeScript**  
   Par exemple, `code.ts`

2. **Écrire ton code dedans**

```ts
const sayHi = () => console.log("Hi");
```

3. **Ouvrir le terminal dans VSC**
    
    - Menu : `Terminal > Nouveau terminal`
        
    - Ou raccourci : `Ctrl + ù` (sur clavier français)
        
4. **Compiler avec la commande suivante** :
```tsc code.ts```

> 📁 Cela génère automatiquement un fichier `code.js` dans le même dossier.

## ⚙️ Ajouter des options de compilation

Tu peux ajouter des options pour choisir la version du JavaScript à générer :

```tsc code.ts --target ES6```

* - `--target` permet de choisir la version JS de sortie : `ES5`, `ES6`, `ES2016`, `ES2020`, etc.

📚 Pour toutes les options disponibles :  
➡️ [https://www.typescriptlang.org/docs/handbook/compiler-options.html](https://www.typescriptlang.org/docs/handbook/compiler-options.html)  
Ou cherche sur Google : `TypeScript CLI options`

✅ Résultat attendu
* Tu tapes `tsc code.ts`
* Tu obtiens automatiquement un fichier **code.js** avec ce contenu :



