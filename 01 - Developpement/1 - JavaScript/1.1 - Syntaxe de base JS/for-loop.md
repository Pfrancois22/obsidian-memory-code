---
tags: [react, juggl]
parent: 
related:
  - foreach
children:
  - map
---

---
title: Opérateur Rest (...) en JavaScript
tags: [javascript, rest, opérateur, débutant]
created: 2025-06-09
---

# Fonction : `for()`

## Description
La fonction `for()` est une structure de contrôle utilisée pour répéter un bloc de code un nombre déterminé de fois. Elle est couramment utilisée dans de nombreux langages de programmation pour itérer sur des ensembles, des listes, des tableaux ou d'autres types de collections.

## Syntaxe Générale


```
for (initialisation; condition; incrémentation) {
    // bloc de code à exécuter
}
```

- **Initialisation** : Déclare et initialise les variables utilisées dans la boucle.
- **Condition** : Évaluée avant chaque itération ; si elle est vraie, le bloc de code s'exécute.
- **Incrémentation** : Modifie les variables après chaque itération.

## Exemples

### Exemple Simple en JavaScript
```javascript
for (let i = 0; i < 5; i++) {
    console.log(i);
}
// Affiche: 0, 1, 2, 3, 4
```


## Utilisations Courantes

- **Itération sur des collections** : Parcourir les éléments d'une liste ou d'un tableau.
- **Opérations répétées** : Exécuter une opération spécifique plusieurs fois.
- **Algorithmes** : Implémenter des algorithmes qui nécessitent une répétition contrôlée.

## Bonnes Pratiques

1. **Limiter la portée des variables** : Déclarez les variables dans l'initialisation si possible pour limiter leur portée au corps de la boucle.
2. **Éviter les modifications inutiles** : Ne modifiez pas les variables d'itération à l'intérieur du bloc sauf si nécessaire.
3. **Utiliser la boucle appropriée** : Assurez-vous que `for()` est le bon choix par rapport à d'autres structures comme `while` ou `do-while

---

## 🔗 Liens connexes

### 📚 Concepts liés

[[foreach]]
### 🛠️ Fiches pratiques
- [[for-loop]]

### 🚧 En cours

