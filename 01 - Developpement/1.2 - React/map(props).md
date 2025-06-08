



# Fiche Technique : map() avec props dans React

## Nom de la fonction  
`map() avec props`

## Définition  
La fonction `map()` permet de parcourir un tableau d'éléments et de retourner un nouveau tableau contenant les résultats du passage de chaque élément par une fonction fournie, souvent utilisée pour générer des composants enfants dans React en passant des propriétés (props).

## Décomposition pas à pas  

1. **Étape 1 :** Créez un tableau de données que vous souhaitez afficher sous forme de composants.
   
2. **Étape 2 :** Utilisez la méthode `map()` sur ce tableau pour itérer sur chaque élément. (voir chaque éléments du tableau)

3. **Étape 3 :** Pour chaque itération, retournez un composant React en lui passant les propriétés (props) nécessaires.

## Exemple d’utilisation  

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

const App = () => {
  const data = [
    { name: 'Apple' },
    { name: 'Banana' },
    { name: 'Cherry' }
  ];

  return <ItemList items={data} />;
};

export default App;
```

### Exemple avec rendu (sortie)  

Si le tableau `data` est fourni comme ci-dessus, le rendu final sera :

- Apple
- Banana
- Cherry

## Liens externes  

- MDN : [Array.prototype.map()](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Array/map)
- W3Schools : [JavaScript Array map() Method](https://www.w3schools.com/jsref/jsref_map.asp)

---

## 🔗 Liens connexes

### 📚 Concepts liés

[[parent::map enfant props]]
[[related::map]]
### 🛠️ Fiches pratiques
- [[map()]]
- [[]]

### 🚧 En cours
- [[]]