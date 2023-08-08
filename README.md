ESLint configuration

## Setup


### EsLint
```
npm install eslint --save-dev

yarn add eslint --dev
```

### Typescript-Eslint/Parser and Typescript-Eslint/Eslint-Plugin
```
npm install @typescript-eslint/parser @typescript-eslint/eslint-plugin --save-dev


yarn add @typescript-eslint/parser @typescript-eslint/eslint-plugin --dev
```

### Standard
```
npm install eslint-config-standard --save-dev

yarn add eslint-config-standard --dev
```

### Eslint-Plugin-React
```
npm install eslint-plugin-react --save-dev

yarn add eslint-plugin-react --dev
```

### Eslint-Plugin-React-Hooks
```
npm install eslint-plugin-react-hooks --save-dev

yarn add eslint-plugin-react-hooks --dev
```

### Eslint-Plugin-Jsx-A11y
```
npm install eslint-plugin-jsx-a11y --save-dev

yarn add eslint-plugin-jsx-a11y --dev
```

### Eslint-Config-Prettier
```
npm install eslint-config-prettier --save-dev

yarn add eslint-config-prettier --dev
```

### Prettier
```
npm install prettier --save-dev

yarn add prettier --dev
```

### @Types/React and @Types/React-Dom (opcional)
```
npm install @types/react @types/react-dom --save-dev

yarn add @types/react @types/react-dom --dev
```

## Inside .eslintrc.json
```
{
  "env": {
    "browser": true,
    "es2021": true,
    "jest": true
  },
  "extends": [
    "plugin:react/recommended",
    "plugin:react-hooks/recommended",
    "plugin:@typescript-eslint/recommended",
    "standard",
    "plugin:prettier/recommended"
  ],
  "parser": "@typescript-eslint/parser",
  "parserOptions": {
    "ecmaFeatures": {
      "jsx": true
    },
    "ecmaVersion": "latest",
    "sourceType": "module"
  },
  "plugins": ["react", "jsx-a11y", "@typescript-eslint"],
  "rules": {
    "prettier/prettier": [
      "error",
      {
        "printWidth": 80,
        "tabWidth": 2,
        "singleQuote": false,
        "trailingComma": "all",
        "arrowParens": "always",
        "semi": true,
        "endOfLine": "auto"
      }
    ],
    "react/react-in-jsx-scope": "off",
    "react/prop-types": "off",
    "jsx-a11y/alt-text": [
      "warn",
      {
        "elements": ["img"],
        "img": ["Image"]
      }
    ],
    "jsx-a11y/aria-props": "warn",
    "jsx-a11y/aria-proptypes": "warn",
    "jsx-a11y/aria-unsupported-elements": "warn",
    "jsx-a11y/role-has-required-aria-props": "warn",
    "jsx-a11y/role-supports-aria-props": "warn"
  },
  "settings": {
    "react": {
      "version": "detect"
    }
  }
}
```

<hr />
<p>Alerrando © 2023 Obrigado por acessar</p>