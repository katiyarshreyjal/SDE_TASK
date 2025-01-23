# React + TypeScript + Vite
Aggriculture Analytics Dashboard
A web application built with React, TypeScript, and Vite to analyze and visualize aggriculture data. The application feature
1. A table displaying crop production extremes by year
2. A bar chart illustrating average crop yields using Apache ECharts.

Features
1. Display crop production extremes(highest and lowest production per year)
2. Show avg crop yields in a bar chart
3. Responsive UI powered by Mantine and styled with its component library
4. Lightweight and fast with vite for development and production builds

Technologies used
1. React - Frontend library for building user interfaces
2. TypeScript - strongly typed programming language for scalability and reliability
3. Mantine - component library for tables and UI styling
4. Apache ECharts - visualization library for creating bar charts
5. Vite - Lightning-fast frontend build tool for modern web development

Prerequisites
1. Node.js(version 16.x)
2. Yarn or npm for package management

Project Structure
task/
├── src/
│   ├── assets/
│   │   └── dataset.json          # JSON dataset for agriculture analytics
│   ├── components/
│   │   ├── BarChart.tsx          # Bar chart component (Apache ECharts)
│   │   └── ProductionTable.tsx   # Table component (Mantine)
│   ├── utils/
│   │   └── dataLoader.ts         # Data processing utility functions
│   ├── App.tsx                   # Main application component
│   ├── main.tsx                  # Entry point of the application
│   └── index.css                 # Global styles
├── public/
│   └── vite.svg                  # Favicon for the app
├── package.json                  # Project configuration and dependencies
└── README.md                     # Project documentation
  
screenshots of project
[Crop Production Extremes]
![img_alt](https://github.com/katiyarshreyjal/SDE_TASK/blob/main/Screenshot%20(605).png?raw=true)
![img_alt](https://github.com/katiyarshreyjal/SDE_TASK/blob/f53e7c9d2a5b0cdb85c76d514f4d5ebc85c8b63c/Screenshot%20(606).png)
![img_alt](https://github.com/katiyarshreyjal/SDE_TASK/blob/80eecfbb6a8b907f43e38885d504bc685640dda1/Screenshot%20(607).png)

[BAR CHART]
![img_alt](https://github.com/katiyarshreyjal/SDE_TASK/blob/c6094d679863e9c77abd92f67c59653255e09c8c/Screenshot%20(608).png)


This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
export default tseslint.config({
  languageOptions: {
    // other options...
    parserOptions: {
      project: ['./tsconfig.node.json', './tsconfig.app.json'],
      tsconfigRootDir: import.meta.dirname,
    },
  },
})
```

- Replace `tseslint.configs.recommended` to `tseslint.configs.recommendedTypeChecked` or `tseslint.configs.strictTypeChecked`
- Optionally add `...tseslint.configs.stylisticTypeChecked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and update the config:

```js
// eslint.config.js
import react from 'eslint-plugin-react'

export default tseslint.config({
  // Set the react version
  settings: { react: { version: '18.3' } },
  plugins: {
    // Add the react plugin
    react,
  },
  rules: {
    // other rules...
    // Enable its recommended rules
    ...react.configs.recommended.rules,
    ...react.configs['jsx-runtime'].rules,
  },
})
```

