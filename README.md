# Browserify and `pnpm` investigation

Steps to reproduce:

```bash
npx pnpm@8.6.2 install
npx pnpm@8.6.2 --filter=@wmartins/frontend build
```

You should see the following error:

```
Error: Can't walk dependency graph: Cannot find module '../../../../../../node_modules/.pnpm/is-buffer@1.1.6/node_modules/is-buffer/index.js' from '../../node_modules/.pnpm/filestack-js@3.26.1_typescript@5.1.3/node_modules/filestack-js/build/browser/filestack.esm.js'
```