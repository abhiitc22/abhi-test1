# Copilot instructions

- Project: a minimal React 19 application built with Vite.
- Entrypoint: `src/main.jsx` creates the React root and renders `src/App.jsx` inside `<StrictMode>`.
- Build flow: `npm run dev`, `npm run build`, `npm run preview`.
- Lint command: `npm run lint` runs ESLint over `**/*.{js,jsx}` using `eslint.config.js`.
- Module format: this repo uses ESM (`package.json` contains `"type": "module"`).
- CSS is imported from JS: `src/App.jsx` imports `./App.css`, and `src/main.jsx` imports `./index.css`.
- Vite config is lightweight: `vite.config.js` only loads `@vitejs/plugin-react`.
- No TypeScript or test runner is configured; do not add TypeScript-only patterns or assume existing tests.
- Static assets: `public/` is served by Vite, while `src/assets/` is for source-managed files.
- JSX note: preserve valid element casing. `src/App.jsx` currently uses `<H1>`; standard DOM tags should be lowercase like `<h1>` unless defining a custom component.
- Avoid inventing cross-service logic; this repository is a single-page front-end app with no backend integration.
- When modifying UI or logic, keep changes small and consistent with the existing app structure: `src/App.jsx` for top-level component logic and `src/main.jsx` for bootstrapping.
