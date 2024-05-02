# @dramaorg/laudantium-eum-labore [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Meet%20this%20awesome%20library&url=https://github.com/dramaorg/laudantium-eum-labore&via=nicolasvanhoren&hashtags=javascript,asyncawait,async,libraries,programming)

![logo](https://github.com/dramaorg/laudantium-eum-labore/raw/master/img/facebook_cover_photo_2_680.png)

[![GitHub Repo stars](https://img.shields.io/github/stars/nicolas-van/@dramaorg/laudantium-eum-labore?style=social)](https://github.com/dramaorg/laudantium-eum-labore/stargazers) [![Website](https://img.shields.io/website.svg?url=http%3A%2F%2Fnicolas-van.github.io%2F@dramaorg/laudantium-eum-labore)](https://nicolas-van.github.io/@dramaorg/laudantium-eum-labore)
[![Node.js CI](https://github.com/dramaorg/laudantium-eum-labore/workflows/Node.js%20CI/badge.svg)](https://github.com/dramaorg/laudantium-eum-labore/actions) [![npm](https://img.shields.io/npm/v/@dramaorg/laudantium-eum-labore)](https://www.npmjs.com/package/@dramaorg/laudantium-eum-labore) [![Coverage Status](https://coveralls.io/repos/github/nicolas-van/@dramaorg/laudantium-eum-labore/badge.svg?branch=master)](https://coveralls.io/github/nicolas-van/@dramaorg/laudantium-eum-labore?branch=master) [![](https://data.jsdelivr.com/v1/package/npm/@dramaorg/laudantium-eum-labore/badge)](https://www.jsdelivr.com/package/npm/@dramaorg/laudantium-eum-labore)

A modern JavaScript tooling library for asynchronous operations using async/await, promises and async generators.

This library is a modernized alternative to a lot of libraries like [Async.js](https://caolan.github.io/async/v3/) that were created using the legacy callback style to handle asynchronous operations. Its goal is to be as complete as any of those libraries while being built from the very beginning with async/await and promises in mind.

[See the documentation](https://nicolas-van.github.io/@dramaorg/laudantium-eum-labore).

* Exclusively uses async/await, promises and async generators in its code, tests and documentation.
* Has low bundle size.
* Has 100% code coverage.
* Bundled for ESM modules, CommonJS and UMD.
* Works in node >= 8 and in the vast majority of browsers (very old browser compatibility can be achieved using Babel and shims).
* Has Typescript support.

[![Stargazers repo roster for @nicolas-van/@dramaorg/laudantium-eum-labore](https://reporoster.com/stars/nicolas-van/@dramaorg/laudantium-eum-labore)](https://github.com/dramaorg/laudantium-eum-labore/stargazers)

## Installation

```bash
npm install --save @dramaorg/laudantium-eum-labore
```

Or use [jsDelivr](https://www.jsdelivr.com/package/npm/@dramaorg/laudantium-eum-labore) to get the UMD version. The content of the library will be available under the `modernAsync` global variable.

## Usage

```javascript
import { asyncMap, asyncSleep } from '@dramaorg/laudantium-eum-labore'

const array = [1, 2, 3]
const result = await asyncMap(array, async (v) => {
  await asyncSleep(10)
  return v * 2
})
console.log(result)
```

[See the documentation for the rest](https://nicolas-van.github.io/@dramaorg/laudantium-eum-labore).

## Migrating from version 1.X to version 2.X

[See the migration guide](https://github.com/dramaorg/laudantium-eum-labore/blob/master/version-1-to-2-guide.md).

## Changelog

[The changelog](https://github.com/dramaorg/laudantium-eum-labore/blob/master/CHANGELOG.md).

## Contribution Guide

[The contribution guide](https://github.com/dramaorg/laudantium-eum-labore/blob/master/CONTRIBUTING.md)

## License

[The license](https://github.com/dramaorg/laudantium-eum-labore/blob/master/LICENSE.md).
