# stringify-author [![NPM version](https://badge.fury.io/js/stringify-author.svg)](http://badge.fury.io/js/stringify-author)


> Stringify an authors object to `name <email> (url)`.

## Install
#### Install with [npm](npmjs.org):

```bash
npm i stringify-author --save-dev
```

## Run tests

```bash
npm test
```

## Usage

```js
var stringify = require('stringify-author');

var authors = stringify({
  name: 'Jon Schlinkert',
  email: 'jon.schlinkert@sellside.com',
  url: 'https://github.com/jonschlinkert'
});

console.log(authors);
//=> 'Jon Schlinkert <jon.schlinkert@sellside.com> (https://github.com/jonschlinkert)'
```

Any of the properties can be used or missing:

```js
var authors = [
  {name: 'Brian Woodward', url: 'https://github.com/doowb'},
  {name: 'Jon Schlinkert', url: 'https://github.com/jonschlinkert'}
];

console.log(authors.map(stringify));
//=> [ 'Brian Woodward (https://github.com/doowb)', 'Jon Schlinkert (https://github.com/jonschlinkert)' ]
```

## Author

**Jon Schlinkert**
 
+ [github/jonschlinkert](https://github.com/jonschlinkert)
+ [twitter/jonschlinkert](http://twitter.com/jonschlinkert) 

## License
Copyright (c) 2014 Jon Schlinkert, contributors.  
Released under the MIT license

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on August 31, 2014._