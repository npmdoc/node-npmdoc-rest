# npmdoc-rest

#### basic api documentation for  [rest (v2.0.0)](https://github.com/cujojs/rest#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-rest.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-rest) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-rest.svg)](https://travis-ci.org/npmdoc/node-npmdoc-rest)

#### RESTful HTTP client library

[![NPM](https://nodei.co/npm/rest.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/rest)

- [https://npmdoc.github.io/node-npmdoc-rest/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-rest/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-rest/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-rest/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-rest/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-rest/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "browser": "./browser",
    "bugs": {
        "url": "https://github.com/cujojs/rest/issues"
    },
    "contributors": [
        {
            "name": "Jeremy Grelle"
        },
        {
            "name": "John Hann",
            "url": "http://unscriptable.com"
        },
        {
            "name": "Michael Jackson",
            "url": "https://github.com/mjackson"
        }
    ],
    "dependencies": {},
    "description": "RESTful HTTP client library",
    "devDependencies": {
        "curl": "https://github.com/cujojs/curl/tarball/0.7.3",
        "poly": "https://github.com/cujojs/poly/tarball/0.5.1",
        "test-support": "~0.4",
        "when": "~3",
        "wire": "~0.9"
    },
    "directories": {},
    "dist": {
        "shasum": "6dfadf66a405c49cfbd5b4bd25b59fd29cd861bc",
        "tarball": "https://registry.npmjs.org/rest/-/rest-2.0.0.tgz"
    },
    "gitHead": "4bd359df2df845eda628d2256fd06bc4a1f5009c",
    "homepage": "https://github.com/cujojs/rest#readme",
    "jspm": {
        "registry": "npm",
        "main": "./browser"
    },
    "keywords": [
        "rest",
        "http",
        "client",
        "rest-template",
        "spring",
        "cujojs"
    ],
    "license": "MIT",
    "main": "./node",
    "maintainers": [
        {
            "name": "scothis"
        }
    ],
    "name": "rest",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/cujojs/rest.git"
    },
    "scripts": {
        "buster": "buster test --node",
        "lint": "jshint .",
        "sauceme": "sauceme",
        "start": "buster static -e browser",
        "test": "npm run-script lint && npm run-script buster",
        "tunnel": "sauceme -m"
    },
    "version": "2.0.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
