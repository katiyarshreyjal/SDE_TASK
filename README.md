# SDE_TASK
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


[BAR CHART]
