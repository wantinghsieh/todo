---
inclusion: always
---

# Tech Stack

> This is a proposed stack for a new project. Nothing is installed yet. Adjust
> any of these choices before building and I will keep the files consistent.

## Language & runtime

- TypeScript
- Node.js (LTS)

## Suggested stack

- **Framework:** React + Vite (frontend) — or adjust if building API-only.
- **Styling:** CSS Modules or Tailwind CSS.
- **State/data:** Local component state to start; introduce a store only when needed.
- **Testing:** Vitest + React Testing Library.
- **Linting/formatting:** ESLint + Prettier.

## Common commands

These are the conventional commands for the suggested stack. They will work once
the project is scaffolded with these tools.

- Install dependencies: `npm install`
- Start dev server: `npm run dev`
- Build for production: `npm run build`
- Run tests once: `npm run test`
- Lint: `npm run lint`

## Conventions

- Use TypeScript strict mode.
- Prefer named exports.
- Keep dependencies minimal; justify each new one.
- Pin dependency versions rather than using open ranges.
