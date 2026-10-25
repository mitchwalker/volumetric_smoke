# volumetric_smoke
A small prototype for volumetric smoke using three.js.

Live demo: https://mitchwalker.github.io/volumetric_smoke/

## Development

The app logic lives in `src/main.ts` and is compiled to `dist/main.js`, which
`index.html` loads. `dist/` is committed so GitHub Pages can serve it directly
with no build step; rebuild and commit it whenever you change the TypeScript.

```sh
npm install
npm run build    # or: npm run watch
```

three.js is loaded at runtime from unpkg via the import map in `index.html`;
the `three` / `@types/three` dev dependencies are only for type checking, so
keep their versions in sync with the import map.
