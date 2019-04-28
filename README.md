# mjs-mocha-bug
Demonstrates a bug in mjs-mocha

`npm test` runs `test/a.test.js` via `mocha`. This passes.

`npm run mjs-test` runs `test/a.test.mjs` via `mjs-mocha`. This fails.

`a.test.js` and `a.test.mjs` are identical except for the `import 'mjs-mocha';` at the top of `a.test.mjs`.
