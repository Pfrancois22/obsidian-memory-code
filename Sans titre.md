

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
