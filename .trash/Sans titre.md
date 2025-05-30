


Génère une fiche au format Markdown sur la fonction **foreach() en React**, en respectant exactement cette structure :
---

# Titre  
Donne le nom de la méthode ou fonction.

# Définition  
Une phrase courte et précise expliquant à quoi sert cette méthode.

# Décomposition pas à pas  
1. Étape 1 : …  
2. Étape 2 : …  
3. Étape 3 : …  
*(énumérer chaque phase de fonctionnement dans l’ordre logique)*

# 3 exemples d’utilisation  
1. **Exemple 1 (basique)**  
   ```jsx
   // code React simple utilisant map()


---

# Titre  
foreach() en React

# Définition  
La méthode `foreach()` en React n'existe pas directement; cependant, elle peut être utilisée via JavaScript pour itérer sur les éléments d'un tableau sans retourner de valeur.

# Décomposition pas à pas  
1. Étape 1 : Importer ou définir le tableau à traiter dans le composant React.
2. Étape 2 : Utiliser la méthode `forEach()` sur ce tableau pour exécuter une fonction donnée sur chaque élément.
3. Étape 3 : Réaliser les actions souhaitées dans le callback fourni à `forEach()`.

# 3 exemples d’utilisation  
1. **Exemple 1 (basique)**  
   ```jsx
   import React from 'react';

   function NumberList() {
     const numbers = [1, 2, 3, 4, 5];
     numbers.forEach((number) => {
       console.log(number);
     });

     return (
       <div>
         Open the console to see the numbers.
       </div>
     );
   }

   export default NumberList;
   ```

2. **Exemple 2 (avec affichage conditionnel)**  
   ```jsx
   import React from 'react';

   function NamesList() {
     const names = ['Alice', 'Bob', 'Charlie'];
     names.forEach((name) => {
       if (name.startsWith('A')) {
         console.log(name);
       }
     });

     return (
       <div>
         Check the console for names starting with A.
       </div>
     );
   }

   export default NamesList;
   ```

3. **Exemple 3 (manipulation DOM simulée)**  
   ```jsx
   import React, { useEffect } from 'react';

   function ItemLogger() {
     const items = ['item1', 'item2', 'item3'];

     useEffect(() => {
       items.forEach((item) => {
         document.body.insertAdjacentHTML('beforeend', `<p>${item}</p>`);
       });
     }, []);

     return (
       <div>
         Items are being logged to the DOM.
       </div>
     );
   }

   export default ItemLogger;
   ```

---