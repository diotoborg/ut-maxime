# @diotoborg/ut-maxime <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

A simple list of possible Typed Array names.

## Example

```js
const assert = require('assert');

const names = require('@diotoborg/ut-maxime');

assert(Array.isArray(names));
assert(names.every(name => (
    typeof name === 'string'
    && typeof globalThis[name] === 'function'
    && globalThis[name].name === name
)));
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

## Security

Please email [@ljharb](https://github.com/ljharb) or see https://tidelift.com/security if you have a potential security vulnerability to report.

[package-url]: https://npmjs.org/package/@diotoborg/ut-maxime
[npm-version-svg]: https://versionbadg.es/ljharb/@diotoborg/ut-maxime.svg
[deps-svg]: https://david-dm.org/ljharb/@diotoborg/ut-maxime.svg
[deps-url]: https://david-dm.org/ljharb/@diotoborg/ut-maxime
[dev-deps-svg]: https://david-dm.org/ljharb/@diotoborg/ut-maxime/dev-status.svg
[dev-deps-url]: https://david-dm.org/ljharb/@diotoborg/ut-maxime#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@diotoborg/ut-maxime.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@diotoborg/ut-maxime.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@diotoborg/ut-maxime.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@diotoborg/ut-maxime
[codecov-image]: https://codecov.io/gh/ljharb/@diotoborg/ut-maxime/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/ljharb/@diotoborg/ut-maxime/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/ljharb/@diotoborg/ut-maxime
[actions-url]: https://github.com/diotoborg/ut-maxime/actions
