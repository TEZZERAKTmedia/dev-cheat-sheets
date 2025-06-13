# 📜 JavaScript / Node.js Cheat Sheet

## 🔧 Package Management
```bash
npm init -y
npm install express
npm run start
```

## 📁 Module Syntax
```js
// CommonJS
const fs = require('fs');

// ES6
import fs from 'fs';
```

## 📡 Fetch & Async
```js
async function getData() {
  const res = await fetch('/api/data');
  const data = await res.json();
}
```

## 🧰 Tools
- `eslint .`
- `npx prettier --write .`
- `npx babel script.js --out-file script.compiled.js`