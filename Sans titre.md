



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
```
tsc code.ts
```

-- 📁 Cela génère automatiquement un fichier `code.js` dans le même dossier.


