# monorepo-experiments

Experimenting with rollup and monorepos for front-end apps.

- "Library" bundles form ES modules and CJS modules.
- "Browser" bundles for UMD bundles packing in their dependencies on ES modules for tree-shaking to occur.

Lerna watch task works great. Editing a library will cause that bundle to rebuild, then that will cause dependant bundles to rebuild, and so-on until the browser bundles are re-built.

