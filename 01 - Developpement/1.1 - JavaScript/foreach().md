---
tags: [react, juggl]
parent: for
related:
  - foreach
children:
  - map
  - map_props
---



# Fonction : foreach()

## Définition
- La fonction `foreach()` permet d'exécuter une fonction donnée sur chaque élément d'un tableau.

## Décomposition pas à pas
1. Étape 1 : Déclarer un tableau contenant les éléments à parcourir.
2. Étape 2 : Appeler la méthode `foreach()` sur ce tableau.
3. Étape 3 : Passer une fonction callback en argument qui sera exécutée pour chaque élément du tableau.

## Exemple d’utilisation

### Exemple 1 (simple)
```javascript
const array = [1, 2, 3, 4, 5];
array.forEach(element => {
    console.log(element);
});


## Liens externes
- MDN : [Array.prototype.forEach() - MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach)
- W3Schools : [JavaScript Array forEach() Method](https://www.w3schools.com/jsref/jsref_foreach.asp)
```

---

## 🔗 Liens connexes

### 📚 Concepts liés

[[map(props)]]
### 🛠️ Fiches pratiques
- [[map()]]


### 🚧 En cours