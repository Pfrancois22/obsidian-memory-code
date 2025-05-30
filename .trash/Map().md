






---




---

# map()

# Définition  
La méthode `map()` est utilisée en React pour itérer sur un tableau et générer un nouvel élément JSX pour chaque élément du tableau.

# Décomposition pas à pas  
1. Étape 1 : Créer un tableau de données que vous souhaitez afficher dans votre composant React.
2. Étape 2 : Utiliser la méthode `map()` sur ce tableau pour transformer chaque élément en un élément JSX.
3. Étape 3 : Retourner le nouveau tableau d'éléments JSX à partir de votre composant, généralement dans la méthode `render()`.

# 3 exemples d’utilisation  
1. **Exemple 1 (basique)**  
   ```jsx
   // code React simple utilisant map()
   import React from 'react';

   function NumberList(props) {
     const numbers = props.numbers;
     const listItems = numbers.map((number) =>
       <li key={number.toString()}>
         {number}
       </li>
     );
     return (
       <ul>{listItems}</ul>
     );
   }

   const numbers = [1, 2, 3, 4, 5];
   ReactDOM.render(
     <NumberList numbers={numbers} />,
     document.getElementById('root')
   );
   ```

2. **Exemple 2 (avec objets)**  
   ```jsx
   // utilisation de map() avec un tableau d'objets
   import React from 'react';

   function UserList(props) {
     const users = props.users;
     const userItems = users.map((user) =>
       <li key={user.id}>
         {user.name} - {user.email}
       </li>
     );
     return (
       <ul>{userItems}</ul>
     );
   }

   const users = [
     { id: 1, name: 'Alice', email: 'alice@example.com' },
     { id: 2, name: 'Bob', email: 'bob@example.com' }
   ];

   ReactDOM.render(
     <UserList users={users} />,
     document.getElementById('root')
   );
   ```

3. **Exemple 3 (avec transformation de données)**  
   ```jsx
   // utilisation de map() pour transformer les données avant l'affichage
   import React from 'react';

   function ProductList(props) {
     const