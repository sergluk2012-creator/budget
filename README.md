# Family Budget Manager — Local Version

This package was prepared for local use. It is based on the exported UIBakery project and adapted to run locally with `json-server` as a fake REST API.

## What was added
- `server/db.json` — empty starter database (users, transactions, categories, budgets, goals)
- `server/routes.json` — simple route mapping for json-server
- `package.json` — scripts to run `dev` and `server` plus dependencies
- `vite.config.ts` — Vite + PWA plugin config

## How to run (step-by-step)

1. Install dependencies:
```bash
npm install
```

2. Run the fake REST API server (json-server):
```bash
npm run server
```
This starts a local API at: `http://localhost:3001`

3. In another terminal, start the app:
```bash
npm run dev
```
Open the app in your browser (usually `http://localhost:5173` or Vite will show the URL).

Alternatively you can run both concurrently (if you installed `concurrently`):
```bash
npm run start
```

## Notes
- The `db.json` file is intentionally empty to act as a clean starter database.
- The app UI and pages from the original export were preserved. If some API endpoints used by the original project point to UIBakery cloud, update fetch/axios base URLs to `http://localhost:3001` in `src` API client files.

Enjoy! 🚀
