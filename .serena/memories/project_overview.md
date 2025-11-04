## Project Purpose
CareforWe is a React single-page application that promotes the CareforWe caregiver-support platform. It contains landing-page style content (home hero, about section, backed-by partners), informational sections (Learn, Contact, Sign In), and utility flows such as newsletter sign-up popups.

## Tech Stack
- React 18 with Vite 5 bundler.
- React Router DOM 6 for page routing.
- Mix of JavaScript (`.jsx`) and TypeScript (`.tsx`) components for context/auth logic.
- Styling via standard CSS files per component plus Tailwind scaffolded config (currently unused).
- Tooling: ESLint (React + hooks rules), Tailwind/PostCSS setup, gh-pages for deployment.

## Codebase Structure
- `src/main.jsx` bootstraps React and wraps the app with router and providers.
- `src/App.jsx` defines top-level routes (`/`, `/learn`, `/contact`, `/signin`, etc.).
- `src/components/` contains feature areas:
  - `home/`, `learn/`, `contact/`, `signin/` for page sections.
  - `navbar/` for navigation variants and styles.
  - `context/` for authentication context/provider (`authContext.tsx`).
  - `util/` for reusable helpers (e.g., `ScrollToTop`, popup modal, `checkAuth.ts`).
- `src/assets/` stores marketing imagery referenced by components.
- `public/` contains the static assets served by Vite.
- Root config: `vite.config.js`, `tailwind.config.js`, `.eslintrc.cjs`, lockfiles, README.

## Notable Guidelines/Patterns
- Components are written as functional React components with hooks (`useState`, `useEffect`, context APIs).
- Routing handled through `<Routes>`/`<Route>` wrappers and `BrowserRouter` in `main.jsx`.
- UI text and layout focused on caregiving resources; popup uses mailchimp-form embed.