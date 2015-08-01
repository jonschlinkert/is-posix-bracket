# is-posix-bracket [![NPM version](https://badge.fury.io/js/is-posix-bracket.svg)](http://badge.fury.io/js/is-posix-bracket)

> Returns true if the given string is a POSIX bracket expression (POSIX character class).

## Install

Install with [npm](https://www.npmjs.com/)

```sh
$ npm i is-posix-bracket --save
```

## Usage

```js
var isPosixBracket = require('is-posix-bracket');

isPosixBracket('[foo:]]');
//=> false
isPosixBracket('[xdigit:]]');
//=> false
isPosixBracket('[[:xdigit:]]');
//=> true
isPosixBracket('[[:xdigit:]]');
//=> true
isPosixBracket('[[:alpha:]123]');
//=> true
isPosixBracket('[[:alpha:]123]');
//=> true
isPosixBracket('[a-c[:digit:]x-z]');
//=> true
isPosixBracket('[:al:]');
//=> true
isPosixBracket('[abc[:punct:][0-9]');
//=> true
```

## Related projects

* [braces](https://github.com/jonschlinkert/braces): Fastest brace expansion for node.js, with the most complete support for the Bash 4.3 braces… [more](https://github.com/jonschlinkert/braces)
* [expand-brackets](https://github.com/jonschlinkert/expand-brackets): Expand POSIX bracket expressions (character classes) in glob patterns.
* [is-glob](https://github.com/jonschlinkert/is-glob): Returns `true` if the given string looks like a glob pattern.
* [is-extglob](https://github.com/jonschlinkert/is-extglob): Returns true if a string has an extglob.
* [micromatch](https://github.com/jonschlinkert/micromatch): Glob matching for javascript/node.js. A drop-in replacement and faster alternative to minimatch and multimatch. Just… [more](https://github.com/jonschlinkert/micromatch)

## Running tests

Install dev dependencies:

```sh
$ npm i -d && npm test
```

## Contributing

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://github.com/jonschlinkert/is-posix-bracket/issues/new)

## Author

**Jon Schlinkert**

+ [github/jonschlinkert](https://github.com/jonschlinkert)
+ [twitter/jonschlinkert](http://twitter.com/jonschlinkert)

## License

Copyright © 2015 Jon Schlinkert
Released under the MIT license.

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on August 01, 2015._