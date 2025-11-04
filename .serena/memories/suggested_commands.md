## Everyday Commands
- Install deps: `npm install` (repo also includes `pnpm-lock.yaml`, but npm scripts are primary).
- Start dev server: `npm run dev` (launches Vite with HMR on http://localhost:5173).
- Type-check/lint JS+TS: `npm run lint`.
- Production build: `npm run build` (outputs to `dist/`).
- Preview build locally: `npm run preview`.
- Deploy to GitHub Pages: `npm run deploy` (runs build then publishes `dist/` via `gh-pages`).

## Useful CLI Tools
- Standard macOS/Darwin utilities: `ls`, `pwd`, `cat`, `find`, `rg` for searches, `git status`.
- Vite DevTools overlay can be toggled via `server.hmr.overlay` in `vite.config.js` if debugging import errors.