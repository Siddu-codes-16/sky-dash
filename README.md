# Skyline Dash

A polished endless 3D runner in the browser. Steer a neon hover-drone through a procedurally built cyberpunk skyline, dodge obstacles, and collect energy orbs.

Stack: **React**, **TypeScript**, **Vite**, **Three.js** (React Three Fiber + Drei), and **Tailwind CSS**. No accounts, API keys, or paid services.






## Controls

- **Steer:** Left / Right arrows, or `A` / `D`
- **Pause:** `Esc` or `P`, or the Pause button
- **Start / resume / restart:** `Enter` or `Space`, or the on-screen buttons
- **Mobile:** Hold the left or right paddles at the bottom of the screen

Score increases over time. Energy orbs add a bonus. Colliding with a pylon, cube, or barrier ends the run. Best score is stored in `localStorage`.

If the system prefers reduced motion, camera sway, sparkles, and extra particles are scaled back.

## Deploy on Vercel

This project uses the default Vite output (`dist/`). `vercel.json` rewrites routes to `index.html`.





## License

MIT
