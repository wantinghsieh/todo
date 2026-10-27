---
inclusion: always
---

# Project Structure

> Proposed layout for a new TypeScript/React Todo app. Update as the real
> structure emerges.

## Top-level layout

```
todo/
├── .kiro/
│   └── steering/        # Project context for Kiro (this folder)
├── src/
│   ├── components/      # Reusable UI components
│   ├── features/        # Feature modules (e.g. tasks/)
│   ├── lib/             # Shared utilities and helpers
│   ├── types/           # Shared TypeScript types
│   ├── App.tsx          # Root component
│   └── main.tsx         # Entry point
├── tests/               # Tests not colocated with source
├── public/              # Static assets
├── index.html
├── package.json
├── tsconfig.json
└── vite.config.ts
```

## Naming conventions

- **Components:** PascalCase files and names — `TaskItem.tsx`.
- **Non-component modules:** camelCase — `taskStore.ts`, `formatDate.ts`.
- **Types/interfaces:** PascalCase — `Task`, `TaskStatus`.
- **Test files:** colocate as `*.test.ts(x)` next to the code they cover.

## Organization patterns

- Group by feature under `src/features/` (e.g. `features/tasks/`), keeping a
  feature's components, hooks, and logic together.
- Put genuinely shared code in `src/lib/` and `src/components/`.
- Keep files focused; split when a file handles more than one responsibility.

## Import conventions

- Use relative imports within a feature.
- Prefer a path alias (e.g. `@/`) for cross-feature imports once configured.
