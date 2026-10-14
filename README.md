# Subscript — yellow-and-black prototype

A standalone mobile subscription-management prototype built with React, TypeScript, and Vite. Bold typography, yellow accents, and Hugeicons support the complete journey from sign-in to updating or recording cancellation of Apple TV.

Live prototype: https://subscript-yellow-prototype.vercel.app

Source: https://github.com/matthieu-pm/subscript-yellow-prototype

## Install and run in one command

Requires Node.js 24 (includes npm) and Git. This repository is public; no GitHub account, sign-in, or GitHub CLI is needed.

From the folder where you keep your projects, paste this command into macOS Terminal, a Linux shell, or Git Bash on Windows:

```sh
git clone https://github.com/matthieu-pm/subscript-yellow-prototype.git && cd subscript-yellow-prototype && npm ci && npm run dev
```

This clones the repository into `subscript-yellow-prototype`, installs the exact locked dependencies, and starts the local app. No environment variables, API keys, or backend setup are needed.

Open the **Local** URL printed in the terminal, usually **http://localhost:5173**. If that port is busy, Vite prints the next available port. Keep the terminal running while using the prototype; press **Ctrl+C** to stop it.

The clone command will stop if a non-empty `subscript-yellow-prototype` folder already exists. It won't overwrite your files. To restart an existing installation instead:

```sh
cd subscript-yellow-prototype
npm run dev
```

To download updates, first save or commit any local edits, then run these commands inside the repository:

```sh
git pull --ff-only
npm ci
npm run dev
```

## Check and build

```sh
npm test
npm run build
```

## Explore

- Sign in with simulated Apple, Google, or email flows. The demo email code is **123456**.
- Set up a profile, connect multiple personal or joint demo accounts, and choose reminder preferences.
- View subscription totals, edit prices and renewal dates, and inspect payment history.
- Apple TV starts at **€120/year**, equivalent to **€10/month**. Recording its cancellation changes the initial total from **€39/month** to **€29/month** while preserving history.
- Manage profile details, connected accounts, notification preferences, and privacy information.
- Use **Explore the demo** to skip setup, or **Reset demo** to restore sample data.

## Prototype boundaries

All data is fictional and anchored to a November 2026 sample snapshot. Authentication, bank connections, provider pages, and reminders are simulated. No credentials are needed, no real payments are made, and cancellation is user-reported. Edits and preferences persist in each browser's local storage.

## Deployment

Vercel builds the repository root with `npm ci` and `npm run build`, then serves `dist`. No environment variables or backend services are required. The `main` branch is the production branch.

This repository contains only the yellow-and-black web prototype. The separate native Revolut-style application and its Git history are not included.
