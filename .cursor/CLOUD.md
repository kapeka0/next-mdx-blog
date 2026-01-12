# Development Environment

## Overview
This is a Next.js blog template using MDX for content, Tailwind CSS for styling, and Turbopack for fast builds.

## Requirements
- Node.js v18.17+
- pnpm (package manager)

## Commands

| Command | Description |
|---------|-------------|
| `pnpm install` | Install dependencies |
| `pnpm dev` | Start development server (port 3000) |
| `pnpm build` | Build for production |
| `npx tsc --noEmit` | TypeScript type checking |

## Key Files
- `app/page.mdx` - Homepage content
- `app/n/*/page.mdx` - Blog posts
- `app/layout.tsx` - Root layout with footer
- `next.config.ts` - Next.js config with MDX setup
- `mdx-components.tsx` - Custom MDX component styling

## Notes
- The database (Postgres) is optional - the app works without `POSTGRES_URL`
- After `pnpm install`, you may need to run `pnpm approve-builds` to approve native dependency builds
- Uses Turbopack for development (experimental)
