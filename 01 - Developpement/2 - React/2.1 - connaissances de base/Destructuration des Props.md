---
title: Destructuration des Props
tags: [javascript, index, navigation]
created: 2025-07-27
---



# Déstructuration & Sécurité des Props (React + TS)

---
 ## liens web
 - [🧾 MDN - Destructuring assignment (React/JS)](https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment)
- [📚 MDN - JSX et props React](https://developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Client-side_JavaScript_frameworks/React_components)
- [📘 W3Schools - React Props](https://www.w3schools.com/react/react_props.asp)
- [📘 W3Schools - JavaScript Destructuring](https://www.w3schools.com/js/js_es6_destructuring.asp)
---

## ✅Déstructuration des Props

Quand tu reçois des props dans un composant, tu dois **déstructurer** chaque champ dont tu as besoin.

```tsx 

type Props = {
  text: string;
  maxLength?: number;
  title?: string;
};

export default function TruncatedText({ text, maxLength = 75, title }: Props) {
  return <p title={title}>{text}</p>;
}
```

* Si tu oublies de sortir `title`, il **ne sera pas utilisé**, même s’il existe dans le type.

## ✅Props Optionnelles avec `?`
```tsx
type Props = {
  title?: string; // ← optionnel
}
```
* Utilise `title || fallback` pour gérer l’absence :
```tsx
<p title={title || "Texte par défaut"}>{text}</p>
```

### 🛡️ Sécurité & Accessibilité

|Élément|Pourquoi ?|Comment faire ?|
|---|---|---|
|`alt` sur image|Accessibilité + fallback|`<img alt="Titre" />`|
|`onError`|Si une image ne se charge pas|`onError={(e) => e.currentTarget.src = "/fallback.jpg"}`|
|`title`|Afficher le texte complet au survol (tooltip)|`title={text}`|
|Ne **pas utiliser** `dangerouslySetInnerHTML` sauf si **validé** par le backend (⚠️ sécurité XSS)|

## 🧪 Exemple Complet :
```tsx
<img
  src={imageUrl || "/fallback.jpg"}
  onError={(e) => { e.currentTarget.src = "/fallback.jpg" }}
  alt={title}
/>

<TruncatedText
  text={description}
  maxLength={75}
  title={description}
/>
```

## 🔗 Liens connexes

- [[1.1 - Syntaxe de base JS/Destructuring]]  ; // rappel de la syntaxe JS pure
- [[2.2 - Syntaxe de base/map_props]] ; // utilisation concrète dans les composants