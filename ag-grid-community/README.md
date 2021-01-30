# cljsjs/ag-grid-community - The JavaScript Datagrid for Enterprise

[](dependency)
```clojure
[cljsjs/ag-grid-community "25.0.1-1"] ;; latest release
```
[](/dependency)

This jar comes with `deps.cljs` as used by the [Foreign Libs][flibs] feature
of the ClojureScript compiler. After adding the above dependency to your project
you can require the packaged library like:

```clojure
(ns application.core
  (:require [cljsjs.ag-grid]))
```

[flibs]: https://clojurescript.org/reference/packaging-foreign-deps

## Upgrading

When upgrading ag-grid, you need to regenerate the externs:
1. Go to https://cdnjs.com/libraries/ag-grid
  (actually, better to use the release from https://github.com/ag-grid/ag-grid/releases)
2. Find the URL for ag-grid.js, such as:

https://cdnjs.cloudflare.com/ajax/libs/ag-grid/25.0.1/ag-grid-community.min.js

3. Go to http://jmmk.github.io/javascript-externs-generator
4. Paste the URL for ag-grid.js and click load.
5. Name the JavaScript object agGrid.
6. Click "Extern!"
7. Copy the JavaScript value to resources/cljsjs/ag-grid-community/common/ag-grid-community.ext.js


https://cdnjs.cloudflare.com/ajax/libs/ag-grid/24.1.0/ag-grid-community.min.js
