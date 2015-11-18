# group-links-by-domain

[![NPM version][npm-image]][npm-url]
[![Build Status][travis-image]][travis-url]
[![Coveralls Status][coveralls-image]][coveralls-url]
[![Dependency Status][depstat-image]][depstat-url]

> group links by domain

## Install

    npm install --save group-links-by-domain

## Usage

```js
import domainLinks from 'group-links-by-domain';

const links = [
  'http://what.ever/a/',
  'http://what.ever/b/',
  'http://foo.bar/1/',
  'http://foo.bar/2/',
  'http://foo.bar/3/'
];

domainLinks(links); /* [
  { domain: 'what.ever',
    links: [
      'http://what.ever/a/',
      'http://what.ever/b/' ]},
  { domain: 'foo.bar',
    links: [
      'http://foo.bar/1/',
      'http://foo.bar/2/',
      'http://foo.bar/3/' ]}
]; */
```

## API

### domainLinks(links)

#### links

*Required*  
Type: `Array` of `String`

Links

## License

MIT © [Vladimir Starkov](https://iamstarkov.com)

[npm-url]: https://npmjs.org/package/group-links-by-domain
[npm-image]: https://img.shields.io/npm/v/group-links-by-domain.svg?style=flat-square

[travis-url]: https://travis-ci.org/iamstarkov/group-links-by-domain
[travis-image]: https://img.shields.io/travis/iamstarkov/group-links-by-domain.svg?style=flat-square

[coveralls-url]: https://coveralls.io/r/iamstarkov/group-links-by-domain
[coveralls-image]: https://img.shields.io/coveralls/iamstarkov/group-links-by-domain.svg?style=flat-square

[depstat-url]: https://david-dm.org/iamstarkov/group-links-by-domain
[depstat-image]: https://david-dm.org/iamstarkov/group-links-by-domain.svg?style=flat-square
