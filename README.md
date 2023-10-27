# Burger-Website-Frontend-Design
# Tailwind Setup

## commands

```commands
npm init -y
npm i -D tailwindcss
npx tailwindcss init
```

## Add configuration in config.js files

```javascript
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./*.{html,js}"],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

## Add the Tailwind directives to your CSS

```javascript
@tailwind base;
@tailwind components;
@tailwind utilities;
```

## Changing package.json file's scripts

```json
{
  "name": "banking-app-with-tailwind",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "build": "tailwindcss -i ./input.css -o ./main/output.css",
    "watch": "tailwindcss -i ./input.css -o ./main/output.css --watch"
  },
  "keywords": [],
  "author": "Moid Alam",
  "license": "ISC",
  "devDependencies": {
    "tailwindcss": "^3.3.4"
  }
}
```

## After changing package.json file's scripts commands and running commands

```commands
npm run build
npm run watch
```
