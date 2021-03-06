# Northbrook ESLint

> Lint your projects with ESLint

# Installation

```sh
npm install --save-dev @northbrook/eslint
```

**northbrook.json**
```js
{
  "plugins": [
    "eslint"
  ]
}
```

# API and configurations

**`northbrook eslint`**

Run ESLint on all of your source code files. Will look for a
`.eslintrc` at the root of your northbrook project, but will fallback
to using `eslint-config-standard`.

### Options

Inside of your `northbrook.json`

```js
{
  "eslint": {
    // default : ['src/']
    "patterns": ["lib/**/*.js"], // paths to lint - supports globs
    // default: 'stylish'
    "formatter": "table" // allows you to specify
  }
}
```
