## Coding Style & Conventions
- Use functional React components with hooks; prefer arrow functions for component declarations and handler callbacks.
- Components live under `src/components/<feature>/` alongside a matching `.css` stylesheet; imports use relative paths.
- Context/state utilities can be written in TypeScript (`.ts`/`.tsx`) while UI components remain `.jsx`; ensure type annotations for public context values.
- Follow ESLint config (`eslint:recommended`, `plugin:react/*`, `react-refresh/only-export-components`)—no unused React components outside exports.
- JSX follows PascalCase component names, camelCase props/handlers, and single quotes inside JSX text only when needed.
- Routing definitions live in `App.jsx`; add new pages as `<Route>` entries and corresponding components.
- Keep imports extension-aware (e.g., `.js`, `.jsx`, `.ts`, `.tsx`) to satisfy Vite when TypeScript files are used.