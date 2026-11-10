# AmberAlert KE

AmberAlert KE is a community-driven web application designed to help raise awareness about missing persons in Kenya and support faster reunification with families.

The platform presents a public-facing landing page, a missing-persons directory, and account flows for sign-up and login. It is built with Nuxt 3 and uses the Nuxt UI component library for the interface.

## Overview

This project focuses on:

- raising awareness about missing children and vulnerable persons
- creating a public-facing community network for reporting and visibility
- making it easier for families, volunteers, and partners to engage with the cause
- supporting later integration with a backend API for user authentication and missing-person records

## Tech stack

- Nuxt 3
- Vue 3
- TypeScript
- Nuxt UI
- Vite

## Project structure

```bash
.
├── app.vue
├── assets/
├── components/
├── pages/
├── public/
├── server/
├── nuxt.config.ts
├── package.json
├── tsconfig.json
├── README.md
└── package-lock.json
```

Key folders:

- `pages/` contains the app routes such as the landing page, home feed, login, signup, partner, and missing person details.
- `components/` contains reusable UI sections like the hero, header, contact block, and home cards.
- `assets/` holds styles and media assets used across the app.
- `server/` is available for Nuxt server-side logic or API helpers.

## Prerequisites

Before running the app, ensure you have:

- Node.js 18 or newer
- npm (or another package manager such as pnpm/yarn/bun)
- a backend API URL if you want auth or records features to work with real data

## Setup

Install dependencies from the project root:

```bash
npm install
```

## Environment configuration

The app reads an optional public API URL from the runtime config:

```bash
API_URL=http://localhost:8000
```

You can expose this in a `.env` file at the project root or pass it through your deployment environment. The project expects this value for API-driven flows such as signup.

## Run the app locally

Start the Nuxt development server:

```bash
npm run dev
```

The application will be available at:

```bash
http://localhost:3000
```

## Production build

Create a production build:

```bash
npm run build
```

Preview the production build locally:

```bash
npm run preview
```

## Notes

- The current codebase is a front-end prototype and UI-focused implementation.
- Some flows, especially authentication and missing-person data handling, are prepared for backend integration.
- If you are connecting to a real backend, make sure the app can reach the correct `API_URL` for your environment.

## Contributing

Contributions are welcome. For feature work or fixes:

1. create a branch for your change
2. make the update
3. run the relevant checks and verify the app works locally
4. open a pull request with a clear summary of the change
