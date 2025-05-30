

# map() dans React avec props

## Définition
La fonction `map()` est utilisée pour itérer sur un tableau et générer une liste de composants React en passant des props à chaque instance.

## Décomposition pas à pas

1. **Étape 1 :** Préparer un tableau contenant les données à afficher.
2. **Étape 2 :** Utiliser la fonction `map()` pour parcourir le tableau.
3. **Étape 3 :** Pour chaque élément du tableau, retourner un composant React avec les données passées en tant que props.

## Exemple d’utilisation

### Exemple 1 (simple)

```jsx
import React from 'react';

const ItemList = ({ items }) => {
  return (
    <ul>
      {items.map((item, index) => (
        <li key={index}>{item.name}</li>
      ))}
    </ul>
  );
};

// Utilisation du composant ItemList
const App = () => {
  const data = [
    { name: 'Item 1' },
    { name: 'Item 2' },
    { name: 'Item 3' }
  ];

  return (
    <div>
      <h1>Liste des éléments</h1>
      <ItemList items={data} />
    </div>
  );
};

export default App;
```

## Liens externes

- MDN : [Array.prototype.map()](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Array/map)
- W3Schools : [JavaScript Array map() Method](https://www.w3schools.com/jsref/jsref_map.asp)
```