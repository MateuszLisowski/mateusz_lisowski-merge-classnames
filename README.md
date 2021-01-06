# @mateusz_lisowski/merge-classnames

[![npm (scoped)](https://img.shields.io/npm/v/@mateusz_lisowski/merge-classnames.svg)](https://www.npmjs.com/package/@mateusz_lisowski/merge-classnames)
[![npm bundle size (minified)](https://img.shields.io/bundlephobia/min/@mateusz_lisowski/merge-classnames.svg)](https://www.npmjs.com/package/@mateusz_lisowski/merge-classnames)

Simple package for merging multiple classes where some of the classes are conditionally applied.

It could be used for example in the React project.

No dependencies.

## Install

```
$ npm install @mateusz_lisowski/merge-classnames
```

## Examples

```js
const cx = require("@mateusz_lisowski/merge-classnames");

cx([{ "any-className": true }, "fixed-class"]); // 'any-className fixed-class'

cx([{ "any-className": false }, { "second-className": true }]); // 'second-className'

cx([{ "any-className": false }, { "second-className": false }]); // ''
```

