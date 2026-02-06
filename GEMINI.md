# GEMINI.md - Project Context for Dra. Ana Benin Site

This file provides the necessary architectural and operational context for Gemini CLI to assist in the development and maintenance of the `abneuro-site` project.

## Project Overview
A professional, medical-focused website for **Dra. Ana Caroline Benin**, a specialist in Neurology and Internal Medicine. The site aims for a clean, professional, and accessible user experience (UX) to showcase medical services, professional background, and clinic location.

### Core Tech Stack
- **Framework:** Vue 3 (Composition API with `<script setup>`).
- **Build Tool:** Vite.
- **Language:** TypeScript.
- **SSG:** `vite-ssg` (Static Site Generation) for optimized performance and SEO.
- **Routing:** `vue-router`.
- **SEO/Meta Management:** `@unhead/vue`.
- **Icons:** Font Awesome (CDN).
- **Styling:** Global CSS variables in `src/assets/main.css` and scoped CSS within components.

## Architecture
- **Entry Point:** `src/main.ts` (uses `ViteSSG`).
- **Main Wrapper:** `src/App.vue` (contains `<TheHeader />`, `<RouterView />`, and `<TheFooter />`).
- **Pages/Views:** Currently centered around `HomeView.vue`.
- **Components:** Modular sections located in `src/components/` (e.g., `TheHero.vue`, `TheServices.vue`, `TheAbout.vue`).
- **Assets:** Global styles, fonts, and images are in `src/assets/`.

## Key Commands
- **Development:** `npm run dev` (Starts Vite dev server).
- **Build (SSG):** `npm run build` (Runs type-check and `vite-ssg build`).
- **Type Checking:** `npm run type-check`.
- **Linting:** `npm run lint` (runs ESLint and oxlint).
- **Formatting:** `npm run format` (runs Prettier).

## Development Conventions
- **Component Naming:** Use `The` prefix for single-instance/global layout components (e.g., `TheHeader.vue`).
- **Script Style:** Always use `<script setup lang="ts">`.
- **Styling:** Prefer CSS variables (defined in `:root` in `main.css`) for consistent colors and spacing.
- **SEO:** Use the `SEO.vue` component or `useHead` directly for route-specific meta tags.
- **Responsiveness:** Ensure mobile-first or highly adaptive designs, as many patients access via mobile.

## TODOs / Ongoing Tasks
- [ ] Font update (Poppins for body, Berdiate for titles) - see `change-fonts.md`.
- [ ] Asset optimization for faster loading.
