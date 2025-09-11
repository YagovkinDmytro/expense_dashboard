# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.

## Importing Components Using Alias @

After configuring your `vite.config.js` with an alias:

```
resolve: {
alias: {
"@": path.resolve(__dirname, "./src"),
},
},
```

you can import components and modules using `@` as a shortcut for the `src/` folder.

### Example

Instead of using long relative paths:

```
import Button from "../../components/Button";
import Dashboard from "../../pages/Dashboard";
```

you can write:

```
import Button from "@/components/Button";
import Dashboard from "@/pages/Dashboard";
```

### Notes:

- `@` points to the `src/` **folder**.
- Works for **JS, JSX, TSX** files inside `src/`.
- You can still use normal relative imports if you prefer.
