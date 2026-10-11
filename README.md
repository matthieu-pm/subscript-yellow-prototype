# Subscript — yellow-and-black prototype

A standalone mobile subscription-management prototype built with React, TypeScript, and Vite. Bold typography, yellow accents, and Hugeicons support the complete journey from sign-in to updating or recording cancellation of Apple TV.

## Run locally

```sh
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
