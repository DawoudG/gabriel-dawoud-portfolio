# Gabriel Dawoud — Portfolio

Personal portfolio website built with React, TypeScript, Vite, and Tailwind CSS.
It presents my background, education, projects, services, and contact
information.

## Run locally

Requirements: Node.js 24 and npm.

```bash
npm install
npm run dev
```

Vite serves the site at <http://localhost:5173>. To create and preview a
production build:

```bash
npm run build
npm run preview
```

## Portfolio sections

- **Home** — welcome message, navigation buttons, and mission statement.
- **About Me** — biography, portrait placeholder, and résumé link.
- **Projects** — three academic projects with project detail pages.
- **Education** — current program, status, expected graduation, and coursework.
- **Services** — software, web, database, and AI/Python development.
- **Contact Me** — contact details and an interactive form that returns to Home.

The résumé is served from `public/resume.pdf`. Replace that file to update the
PDF while keeping the About page link unchanged.

## Project structure

```text
public/                 Static files, including resume.pdf and the SPA fallback
src/assets/             Portfolio illustrations
src/components/         Shared navigation, footer, logo, and About components
src/data/projects.ts    Shared project data for cards and detail pages
src/pages/              Page components
src/styles/index.css    Tailwind imports, theme tokens, and shared styles
```

## Deployment

Run `npm run build` and deploy the generated `dist/` directory to a static
hosting provider. The included GitHub Actions workflow deploys to Netlify when
the required `NETLIFY_SITE_ID` and `NETLIFY_AUTH_TOKEN` repository secrets are
configured.

## Scripts

| Command | Description |
| --- | --- |
| `npm run dev` | Start the Vite development server. |
| `npm run typecheck` | Run TypeScript checks without emitting files. |
| `npm run build` | Type-check and create a production build in `dist/`. |
| `npm run preview` | Serve the production build locally. |
