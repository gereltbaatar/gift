# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

- `npm run dev` - Start development server at localhost:3000
- `npm run build` - Build for production
- `npm run lint` - Run ESLint

## Architecture

This is a Next.js 16 project using the App Router pattern with React 19.

**Key technologies:**
- Tailwind CSS v4 (uses `@import "tailwindcss"` syntax in CSS)
- TypeScript with strict mode
- ESLint with Next.js core-web-vitals and TypeScript configs

**Path alias:** `@/*` maps to the project root

**Styling approach:** Tailwind CSS with CSS custom properties for theming. Theme colors are defined in `app/globals.css` using `@theme inline` for Tailwind integration. Dark mode uses `prefers-color-scheme` media query.

**Fonts:** Geist and Geist Mono loaded via `next/font/google`, exposed as CSS variables `--font-geist-sans` and `--font-geist-mono`.
