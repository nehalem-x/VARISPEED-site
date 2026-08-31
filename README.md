# VARISPEED — presentation site

Standalone presentation website for
[nehalem-x/VARISPEED](https://github.com/nehalem-x/VARISPEED). It can be cloned
independently or kept in the `website/` directory of the main project. The
repository contains no deployment configuration and runs locally by default.

## Development

```bash
npm ci
npm run dev
```

Open the local address printed by the development server (normally
`http://localhost:3000`).

Quality checks:

```bash
npm run lint
npx tsc --noEmit
npm run build
npm audit --omit=dev
```

The interactive graph reuses the production `GraphEngine` from VARISPEED. The
hero particle field is a local Three.js shader and respects reduced-motion and
page visibility preferences.
