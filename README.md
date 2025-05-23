# React + Vite

This template provides a minimal setup to get **React** working in **Vite** with **Hot Module Replacement (HMR)** and some basic **ESLint** rules. It is a simple, efficient starting point for building modern React apps with Vite.

## Official Plugins Available

Currently, two official plugins are available for React in Vite:

1. **[@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md)**  
   - Uses **Babel** for Fast Refresh, enabling quick component updates during development.
   
2. **[@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc)**  
   - Uses **SWC** for Fast Refresh, offering a faster alternative to Babel for modern React projects.

## Expanding the ESLint Configuration

If you are developing a **production application**, it’s highly recommended to use **TypeScript** and enable **type-aware lint rules** to improve code quality and prevent common issues.

To integrate TypeScript and **`typescript-eslint`**, check out the [TypeScript template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) which is pre-configured with TypeScript and ESLint for optimal development.

### TypeScript Integration

1. To add TypeScript to your project, follow the instructions in the **TypeScript template**.
2. You can also configure **`typescript-eslint`** for type-aware linting by installing and setting up the following dependencies:

```bash
npm install --save-dev @typescript-eslint/parser @typescript-eslint/eslint-plugin

And update your .eslintrc.js configuration to use the typescript-eslint plugin.
Recommended ESLint Rules for Production

If you're using TypeScript, here are some recommended linting rules to enable for better code quality:

{
  "extends": ["eslint:recommended", "plugin:react/recommended", "plugin:@typescript-eslint/recommended"],
  "parser": "@typescript-eslint/parser",
  "plugins": ["react", "@typescript-eslint"],
  "rules": {
    "@typescript-eslint/explicit-module-boundary-types": "warn",
    "react/jsx-uses-react": "off",
    "react/react-in-jsx-scope": "off"
  }
}

Resources

    Vite Documentation
    React Documentation
    Babel Documentation
    SWC Documentation
    TypeScript Documentation
    typescript-eslint Documentation
