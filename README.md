## [![npm][npmjs-img]][npmjs-url] [![standard style][standard-img]][standard-url] [![build status][travis-img]][travis-url] [![coverage status][coveralls-img]][coveralls-url] [![deps status][daviddm-img]][daviddm-url]

> Parse default `git log` style to array of objects from git repository of current working directory or given filepath

## Install
```
npm i parse-git-log --save
npm test
```


## Usage
> For more use-cases see the [tests](./test.js)

```js
var parseGitLog = require('parse-git-log');

parseGitLog(function(err, data) {
  var json = JSON.stringify(data, null, 2)
  console.log(json)
  //=> array of objects
  //  [{
  //     "message": "Release v1.0.0",
  //     "commit": "0d31dc3827c7c979a9732425e18fcdb17596b737",
  //     "author": "tunnckoCore <mameto_100@mail.bg>",
  //     "date": "Fri Apr 10 16:32:50 2015 +0300"
  //   },
  //   {
  //     "message": "run update, close #1",
  //     "commit": "0d0433d45456f2a35c01d534ecd0796eb57a4317",
  //     "author": "tunnckoCore <mameto_100@mail.bg>",
  //     "date": "Fri Apr 10 16:24:53 2015 +0300"
  //   },
  //   {
  //     "message": "first commits",
  //     "commit": "e97427979b8580cdbc211f05dfe85a336eae2d75",
  //     "author": "tunnckoCore <mameto_100@mail.bg>",
  //     "date": "Tue Apr 7 13:22:42 2015 +0300"
  //   }]
})
```


## Author
**Charlike Mike Reagent**
+ [gratipay/tunnckoCore][author-gratipay]
+ [twitter/tunnckoCore][author-twitter]
+ [github/tunnckoCore][author-github]
+ [npmjs/tunnckoCore][author-npmjs]
+ [more ...][contrib-more]


## License [![MIT license][license-img]][license-url]
Copyright (c) 2015 [Charlike Mike Reagent][contrib-more], [contributors][contrib-graf].  
Released under the [`MIT`][license-url] license.


[npmjs-url]: http://npm.im/parse-git-log
[npmjs-img]: https://img.shields.io/npm/v/parse-git-log.svg?style=flat&label=parse-git-log

[coveralls-url]: https://coveralls.io/r/tunnckoCore/parse-git-log?branch=master
[coveralls-img]: https://img.shields.io/coveralls/tunnckoCore/parse-git-log.svg?style=flat

[license-url]: https://github.com/tunnckoCore/parse-git-log/blob/master/LICENSE.md
[license-img]: https://img.shields.io/badge/license-MIT-blue.svg?style=flat

[travis-url]: https://travis-ci.org/tunnckoCore/parse-git-log
[travis-img]: https://img.shields.io/travis/tunnckoCore/parse-git-log.svg?style=flat

[daviddm-url]: https://david-dm.org/tunnckoCore/parse-git-log
[daviddm-img]: https://img.shields.io/david/tunnckoCore/parse-git-log.svg?style=flat

[author-gratipay]: https://gratipay.com/tunnckoCore
[author-twitter]: https://twitter.com/tunnckoCore
[author-github]: https://github.com/tunnckoCore
[author-npmjs]: https://npmjs.org/~tunnckocore

[contrib-more]: http://j.mp/1stW47C
[contrib-graf]: https://github.com/tunnckoCore/parse-git-log/graphs/contributors

[standard-url]: https://github.com/feross/standard
[standard-img]: https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat

***

_Proudly generated by [docks(1)](https://github.com/tunnckoCore/docks), May 7, 2015_