---
title: Destructuration des Props
tags: [javascript, index, navigation]
created: 2025-07-27
---  

# Déstructuration & Sécurité des Props (React + TS)

## Déstructuration des Props

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

## Props Optionnelles avec `?`
```tsx
type Props = {
  title?: string; // ← optionnel
}
```
* Utilise `title || fallback` pour gérer l’absence :
* 