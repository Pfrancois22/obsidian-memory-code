


[[map(props)]]

# Fonction: map() en React

## Définition
La fonction `map()` est utilisée pour itérer sur des tableaux et transformer chaque élément selon une fonction donnée, retournant un nouveau tableau.

## Décomposition pas à pas
1. **Étape 1** : Créez un tableau de données à manipuler.
2. **Étape 2** : Appliquez la méthode `map()` sur ce tableau en passant une fonction de transformation comme argument.
3. **Étape 3** : Utilisez le tableau résultant, par exemple pour générer des éléments JSX dans un composant React.

## Exemple d’utilisation
### Exemple 1 (simple)
```jsx
import React from 'react';

const NumberList = () => {
  const numbers = [1, 2, 3, 4, 5];
  const listItems = numbers.map((number) => <li key={number.toString()}>{number}</li>);

  return <ul>{listItems}</ul>;
};

export default NumberList;
```

## Liens externes
- MDN : [Array.prototype.map()](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Array/map)
- W3Schools : [JavaScript Array map()](https://www.w3schools.com/jsref/jsref_map.asp)


---

## 🔗 Liens connexes

### 📚 Concepts liés
- [[map(props)]]
- [[map()]]

### 🛠️ Fiches pratiques
- [[Transcompiler TypeScript avec VSC]]
- [[Utiliser le watch mode de TypeScript]]

### 🚧 En cours
- [[Fiche à créer - Compiler TS avec tsconfig.json]]