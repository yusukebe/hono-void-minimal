# hono-void-minimal

Hono + hono/jsx on [Void](https://void.cloud). No React.

```sh
pnpm install
pnpm dev
```

```sh
pnpm deploy
```

Add a file to `routes/` to add an endpoint:

```tsx
// routes/about.tsx → GET /
import { defineHandler } from 'void'

export const GET = defineHandler((c) => {
  return c.html(<h1>I'm Hono</h1>)
})
```

Docs: `node_modules/void/docs/`
