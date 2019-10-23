# Pre commit 

## configuración
se intalaran los paquetes **husky** y **lint-staged**

## Intalar: 

```bash
npm install --save-dev husky lint-staged
```


```json
"lint-staged": {
    "*.{js,css,json,md}": [
      "eslint --fix",
      "prettier --write",
      "git add"
    ]
  }
```

```javascript
// package.json

"scripts": {
	"precommit": "lint-staged",
},

```


