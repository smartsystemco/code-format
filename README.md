# Code Format

Foobar is a Python library for dealing with word pluralization.

## Installation Husky

1. Install [husky](https://typicode.github.io/husky)

```
npm install husky --save-dev
```

2. Enable Git hooks

```
npx husky install
```

3. Create a hook

```
npx husky add .husky/pre-commit "npm run format"
```

## Installation Prettier

1. Install [prettier](https://prettier.io/)

```
npm install prettier --save-dev
```

## Package.json

add below lines to "scripts" section

```json
"scripts": {
    "lint": "prettier --check .",
    "format": "prettier --write ."
},
```

## Prettier Config

1. to avoid exceptions

#### .prettierignore

```
node_modules
test
```

2. to custom setting

#### .prettierrc.json

```json
{
	"tabWidth": 2,
	"useTabs": true,
	"printWidth": 80,
	"semi": true,
	"trailingComma": "es5",
	"jsxSingleQuote": true,
	"singleQuote": true
}
```

