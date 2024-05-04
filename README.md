# @bobyzgirlllnpm/placeat-dignissimos-quae <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Is this value a JS Map? This module works cross-realm/iframe, and despite ES6 @@toStringTag.

## Example

```js
var isMap = require('@bobyzgirlllnpm/placeat-dignissimos-quae');
assert(!isMap(function () {}));
assert(!isMap(null));
assert(!isMap(function* () { yield 42; return Infinity; });
assert(!isMap(Symbol('foo')));
assert(!isMap(1n));
assert(!isMap(Object(1n)));

assert(!isMap(new Set()));
assert(!isMap(new WeakSet()));
assert(!isMap(new WeakMap()));

assert(isMap(new Map()));

class MyMap extends Map {}
assert(isMap(new MyMap()));
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@bobyzgirlllnpm/placeat-dignissimos-quae
[npm-version-svg]: https://versionbadg.es/inspect-js/@bobyzgirlllnpm/placeat-dignissimos-quae.svg
[deps-svg]: https://david-dm.org/inspect-js/@bobyzgirlllnpm/placeat-dignissimos-quae.svg
[deps-url]: https://david-dm.org/inspect-js/@bobyzgirlllnpm/placeat-dignissimos-quae
[dev-deps-svg]: https://david-dm.org/inspect-js/@bobyzgirlllnpm/placeat-dignissimos-quae/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@bobyzgirlllnpm/placeat-dignissimos-quae#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@bobyzgirlllnpm/placeat-dignissimos-quae.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@bobyzgirlllnpm/placeat-dignissimos-quae.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@bobyzgirlllnpm/placeat-dignissimos-quae.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@bobyzgirlllnpm/placeat-dignissimos-quae
[codecov-image]: https://codecov.io/gh/inspect-js/@bobyzgirlllnpm/placeat-dignissimos-quae/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@bobyzgirlllnpm/placeat-dignissimos-quae/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@bobyzgirlllnpm/placeat-dignissimos-quae
[actions-url]: https://github.com/bobyzgirlllnpm/placeat-dignissimos-quae/actions
