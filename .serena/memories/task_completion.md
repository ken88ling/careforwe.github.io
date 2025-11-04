## Task Completion Checklist
1. Ensure `npm run lint` passes to catch React/JS issues per ESLint config.
2. Run `npm run build` to verify the Vite production bundle succeeds (this also exercises Tailwind/PostCSS).
3. If routing or deploy behavior changed, optionally `npm run preview` before committing.
4. For deploy-related work, run `npm run deploy` or instruct the user accordingly (publishes to GitHub Pages via `gh-pages`).
5. Review affected components/screens manually in `npm run dev` to confirm styling and navigation since there are no automated tests.