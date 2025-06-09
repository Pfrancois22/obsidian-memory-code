

# Plugin VSC : ESLint

* ESLint est un plugin qui permet de respecter TypScript

 ## Configuration
Dans la configuration, on peu lui mettre des Rules (règles).


```rules: {

      ...reactHooks.configs.recommended.rules,

      'react-refresh/only-export-components': [

        'warn',

        { allowConstantExport: true },

      ],

    },
```

* Règles qui peux être utiles
sur le site [[palantir.github.io/tslint/rules/]]

[[https://palantir.github.io/tslint/rules/no-console/]]

cela permet de corriger (enlever) tous les console.log

> Pour tester le code, 