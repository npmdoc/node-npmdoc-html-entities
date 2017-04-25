# npmdoc-html-entities

#### basic api documentation for  [html-entities (v1.2.1)](https://github.com/mdevils/node-html-entities#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-html-entities.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-html-entities) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-html-entities.svg)](https://travis-ci.org/npmdoc/node-npmdoc-html-entities)

#### Faster HTML entities encode/decode library.

[![NPM](https://nodei.co/npm/html-entities.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/html-entities)

- [https://npmdoc.github.io/node-npmdoc-html-entities/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-html-entities/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-html-entities/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-html-entities/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-html-entities/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-html-entities/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Marat Dulin"
    },
    "bugs": {
        "url": "https://github.com/mdevils/node-html-entities/issues"
    },
    "dependencies": {},
    "description": "Faster HTML entities encode/decode library.",
    "devDependencies": {
        "chai": "^1.9.1",
        "coveralls": "^2.11.2",
        "entities": "*",
        "mocha": "^1.21.4",
        "node-html-encoder": "*",
        "unit-coverage": "^3.0.1"
    },
    "directories": {},
    "dist": {
        "shasum": "0df29351f0721163515dfb9e5543e5f6eed5162f",
        "tarball": "https://registry.npmjs.org/html-entities/-/html-entities-1.2.1.tgz"
    },
    "engines": [
        "node >= 0.4.0"
    ],
    "files": [
        "index.js",
        "lib",
        "LICENSE"
    ],
    "gitHead": "dc08bde42ee6468d60ca617061b0b37b2edc45ca",
    "homepage": "https://github.com/mdevils/node-html-entities#readme",
    "keywords": [
        "html",
        "html entities",
        "html entities encode",
        "html entities decode",
        "entities",
        "entities encode",
        "entities decode"
    ],
    "license": "MIT",
    "main": "index",
    "maintainers": [
        {
            "name": "mdevils"
        }
    ],
    "name": "html-entities",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mdevils/node-html-entities.git"
    },
    "scripts": {
        "benchmark": "node benchmark/benchmark",
        "coverage": "unit-coverage run -p common",
        "coverage-html": "unit-coverage run -p common -r html -o coverage.html",
        "test": "mocha --recursive -R spec test",
        "travis": "npm test && unit-coverage run -p common -r lcov -o coverage.lcov && cat coverage.lcov | coveralls"
    },
    "unit-coverage": {
        "common": [
            "-s",
            "lib/**/*.js",
            "-t",
            "test/**/*.js"
        ]
    },
    "version": "1.2.1",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
