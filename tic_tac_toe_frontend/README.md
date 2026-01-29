# Modern Tic Tac Toe (React)

Simple two-player Tic Tac Toe game with a modern, responsive UI.

## Tech stack

- **React** (latest supported by this project)
- **Create React App (CRA)** (detected via `react-scripts` in `package.json`)
- **Styling**: Vanilla CSS (see `src/App.css`, `src/index.css`)

## Getting started

From the `tic_tac_toe_frontend` directory:

### Install

```bash
npm install
```

### Run (development)

```bash
npm start
```

The dev server will run on (default): `http://localhost:3000`

### Build (production)

```bash
npm run build
```

### Test

```bash
npm test
```

## Environment variables

This app uses Create React App environment variables (must be prefixed with `REACT_APP_`).

The following variables exist in `.env`:

- `REACT_APP_API_BASE` (optional): Base URL for API requests.
- `REACT_APP_BACKEND_URL` (optional): Backend service URL (often same as API base).
- `REACT_APP_FRONTEND_URL` (optional): Public URL for this frontend (used for links/redirects if needed).
- `REACT_APP_WS_URL` (optional): WebSocket URL for real-time features (if used).
- `REACT_APP_NODE_ENV` (optional): Environment label (e.g., `development`).
- `REACT_APP_NEXT_TELEMETRY_DISABLED` (optional): Disables telemetry (kept for compatibility with tooling).
- `REACT_APP_ENABLE_SOURCE_MAPS` (optional): Toggle source map generation.
- `REACT_APP_PORT` (optional): Preferred port for the dev server.
- `REACT_APP_TRUST_PROXY` (optional): Whether to trust proxy headers (relevant in proxied deployments).
- `REACT_APP_LOG_LEVEL` (optional): Client log verbosity (e.g., `info`, `debug`).
- `REACT_APP_HEALTHCHECK_PATH` (optional): Path used for health checks (e.g., `/healthz`).
- `REACT_APP_FEATURE_FLAGS` (optional): Feature flags (JSON string).
- `REACT_APP_EXPERIMENTS_ENABLED` (optional): Toggle experimental UI/features.

## Project structure

Key folders/files:

- `public/` – Static assets and HTML template
- `src/` – Application source code
  - `src/index.js` – App entry point
  - `src/App.js` – Main app component
  - `src/App.css` / `src/index.css` – Global and app styling
  - `src/setupTests.js` – Testing setup (Jest + Testing Library)

## Development notes

- **Coding standards**: React (modern functional components), hooks (`useState`, `useEffect`), and idiomatic JSX.
- **Theme/style guide** (light theme):
  - Primary: `#3b82f6`
  - Success/accent: `#06b6d4`
  - Background: `#f9fafb`
  - Surface: `#ffffff`
  - Text: `#111827`

### Previewing the production build

```bash
npm run build
npx serve -s build
```

## License

MIT
