# DevScot Digital Agency Website

A Next.js 15 App Router site scaffold for the DevScot agency, set up with React 19, TypeScript and Tailwind CSS v4. The agency content is not written yet; the home page is still the starter template.

## The problem

An agency site has to explain what the studio builds and make it easy for a prospective client to get in touch. This repo is the foundation for that site: routing, fonts, styling and build tooling are in place, and the page content is the next piece.

## What it does

What the code does today:

- Renders a root layout (`app/layout.tsx`) that loads Geist Sans and Geist Mono through `next/font` and sets the page metadata.
- Serves a single home page (`app/page.tsx`) that still contains the create-next-app starter content.
- Styles with Tailwind CSS v4 utility classes, plus CSS variables for light and dark colour schemes in `app/globals.css`.
- Ships static SVG assets in `public/` and uses `next/image` for the logo.
- Runs lint through `next lint`.

## How it's built

- **Framework**: Next.js 15.5 with the App Router. `pnpm dev` runs Turbopack.
- **UI**: React 19.2 and TypeScript 5.
- **Styling**: Tailwind CSS v4 through `@tailwindcss/postcss` (`postcss.config.mjs`).
- **Fonts and images**: `next/font` for Geist, `next/image` for the logo, both handled by the framework.


## Running it locally

Requires Node.js 20 or newer. `pnpm` is recommended.

```bash
pnpm install
pnpm dev
```

Open http://localhost:3000.

Other scripts: `pnpm build`, `pnpm start`, `pnpm lint`.

## What I learned / what I'd do next

- Replace the starter page with the agency content. The metadata title and description still read "Create Next App".
- Add the services, case studies and contact form that the old README described. None of them are in the code yet.
- There are no tests. Add at least a smoke test for the home page once the content exists.

## Author

Created by [Mehfooz-ur-Rehman](https://github.com/MehfoozurRehman).
