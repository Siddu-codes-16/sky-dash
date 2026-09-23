# Skyline Dash

A polished endless 3D runner in the browser. Steer a neon hover-drone through a procedurally built cyberpunk skyline, dodge obstacles, and collect energy orbs.

Stack: **React**, **TypeScript**, **Vite**, **Three.js** (React Three Fiber + Drei), and **Tailwind CSS**. No accounts, API keys, or paid services.

## Local setup

Needs Node.js 20+ and npm.

```bash
git clone <your-repo-url> skyline-dash
cd skyline-dash
npm install
npm run dev
```

Open the URL Vite prints (usually `http://localhost:5173`).

## Scripts

| Command | What it does |
| --- | --- |
| `npm run dev` | Start the Vite dev server |
| `npm run build` | Type-check and build production files into `dist/` |
| `npm run preview` | Serve the production build locally |
| `npm run lint` | Run oxlint |

## Controls

- **Steer:** Left / Right arrows, or `A` / `D`
- **Pause:** `Esc` or `P`, or the Pause button
- **Start / resume / restart:** `Enter` or `Space`, or the on-screen buttons
- **Mobile:** Hold the left or right paddles at the bottom of the screen

Score increases over time. Energy orbs add a bonus. Colliding with a pylon, cube, or barrier ends the run. Best score is stored in `localStorage`.

If the system prefers reduced motion, camera sway, sparkles, and extra particles are scaled back.

## Deploy on Vercel

This project uses the default Vite output (`dist/`). `vercel.json` rewrites routes to `index.html`.

### Option A — Vercel dashboard

1. Push the repo to GitHub, GitLab, or Bitbucket.
2. Go to [vercel.com](https://vercel.com) and import the project.
3. Keep the defaults:
   - **Framework Preset:** Vite
   - **Build Command:** `npm run build`
   - **Output Directory:** `dist`
   - **Install Command:** `npm install`
4. Deploy. No environment variables are required.

### Option B — Vercel CLI

```bash
npm install -g vercel
cd skyline-dash
npm run build
vercel
```

For production:

```bash
vercel --prod
```

## License

MIT
