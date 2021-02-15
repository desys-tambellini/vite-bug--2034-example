Vite Bug Test Project

* `npm i`
* open `src/App.vue`
* `npm run build` and the build goes fine
* uncomment from line 12 to 14
* `npm run build` and it will throw an error

```
$ vite build --ssr src/entry-server.js --outDir dist/server
building SSR bundle for production...
✓ 2 modules transformed.
[rollup-plugin-dynamic-import-variables] Identifier '_imports_0' has already been declared (5:7)
file: C:/Users/s.tambellini/Downloads/vite-bug-example/src/App.vue:5:7
error during build:
SyntaxError: Identifier '_imports_0' has already been declared (5:7)
    at Object.pp$4.raise (C:\Users\s.tambellini\Downloads\vite-bug-example\node_modules\rollup\dist\shared\rollup.js:15849:13)
    at Object.pp$5.declareName (C:\Users\s.tambellini\Downloads\vite-bug-example\node_modules\rollup\dist\shared\rollup.js:15923:26)
    at Object.pp$2.checkLValSimple (C:\Users\s.tambellini\Downloads\vite-bug-example\node_modules\rollup\dist\shared\rollup.js:14739:48)
    at Object.pp$1.parseImportSpecifiers (C:\Users\s.tambellini\Downloads\vite-bug-example\node_modules\rollup\dist\shared\rollup.js:14428:10)
    at Object.pp$1.parseImport (C:\Users\s.tambellini\Downloads\vite-bug-example\node_modules\rollup\dist\shared\rollup.js:14412:28)
    at Object.pp$1.parseStatement (C:\Users\s.tambellini\Downloads\vite-bug-example\node_modules\rollup\dist\shared\rollup.js:13715:47)
    at Object.pp$1.parseTopLevel (C:\Users\s.tambellini\Downloads\vite-bug-example\node_modules\rollup\dist\shared\rollup.js:13598:21)
    at Object.parse (C:\Users\s.tambellini\Downloads\vite-bug-example\node_modules\rollup\dist\shared\rollup.js:13400:15)
    at Function.parse (C:\Users\s.tambellini\Downloads\vite-bug-example\node_modules\rollup\dist\shared\rollup.js:13421:35)
    at Object.Graph.contextParse [as parse] (C:\Users\s.tambellini\Downloads\vite-bug-example\node_modules\rollup\dist\shared\rollup.js:19126:70)

```
