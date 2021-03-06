# to-object-path-js [![NPM version](https://img.shields.io/npm/v/to-object-path-js.svg?style=flat)](https://www.npmjs.com/package/to-object-path-js) [![NPM monthly downloads](https://img.shields.io/npm/dm/to-object-path-js.svg?style=flat)](https://npmjs.org/package/to-object-path-js)  [![NPM total downloads](https://img.shields.io/npm/dt/to-object-path-js.svg?style=flat)](https://npmjs.org/package/to-object-path-js) [![Linux Build Status](https://img.shields.io/travis/oronnadiv/to-object-path.svg?style=flat&label=Travis)](https://travis-ci.org/oronnadiv/to-object-path)

#### This is a fork of the [package](https://github.com/jonschlinkert/to-object-path) created by [Jon Schlinkert](https://github.com/jonschlinkert). The original package has not been updated for several years and has multiple security vulnerabilities.  Creating this fork was the only way to address them. Read this [issue](https://github.com/jonschlinkert/to-object-path/issues/3#issuecomment-752862800) for more information.

> Create an object path from a list or array of strings.

## Install

Install with [npm](https://www.npmjs.com/)

```sh
$ npm i to-object-path-js --save
```

## Usage

```js
var toPath = require('to-object-path-js');

toPath('foo', 'bar', 'baz');
toPath('foo', ['bar', 'baz']);
//=> 'foo.bar.baz'
```

Also supports passing an arguments object (without having to slice args):

```js
function foo() {
  return toPath(arguments);
}

foo('foo', 'bar', 'baz');
foo('foo', ['bar', 'baz']);
//=> 'foo.bar.baz'
```

Visit the [example](./example.js) to see how this could be used in an application.

## Related projects

* [get-value](https://www.npmjs.com/package/get-value): Use property paths (`  a.b.c`) to get a nested value from an object. | [homepage](https://github.com/jonschlinkert/get-value)
* [has-value](https://www.npmjs.com/package/has-value): Returns true if a value exists, false if empty. Works with deeply nested values using… [more](https://www.npmjs.com/package/has-value) | [homepage](https://github.com/jonschlinkert/has-value)
* [omit-value](https://www.npmjs.com/package/omit-value): Omit properties from an object or deeply nested property of an object using object path… [more](https://www.npmjs.com/package/omit-value) | [homepage](https://github.com/jonschlinkert/omit-value)
* [set-value](https://www.npmjs.com/package/set-value): Create nested values and any intermediaries using dot notation (`'a.b.c'`) paths. | [homepage](https://github.com/jonschlinkert/set-value)
* [unset-value](https://www.npmjs.com/package/unset-value): Delete nested properties from an object using dot notation. | [homepage](https://github.com/jonschlinkert/unset-value)

## Running tests

Install dev dependencies:

```sh
$ npm i -d && npm test
```

## Contributing

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://github.com/OronNadiv/to-object-path/issues/new).

## Author

**Oron Nadiv**

+ [github/OronNadiv](https://github.com/OronNadiv)

**Jon Schlinkert**

+ [github/jonschlinkert](https://github.com/jonschlinkert)
+ [twitter/jonschlinkert](http://twitter.com/jonschlinkert)
