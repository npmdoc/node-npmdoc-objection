# npmdoc-objection

#### api documentation for  objection (v0.7.12)  [![npm package](https://img.shields.io/npm/v/npmdoc-objection.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-objection) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-objection.svg)](https://travis-ci.org/npmdoc/node-npmdoc-objection)

#### An SQL-friendly ORM for Node.js

[![NPM](https://nodei.co/npm/objection.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/objection)

- [https://npmdoc.github.io/node-npmdoc-objection/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-objection/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-objection/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-objection/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-objection/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-objection/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "objection",
    "version": "0.7.12",
    "description": "An SQL-friendly ORM for Node.js",
    "main": "lib/objection.js",
    "license": "MIT",
    "scripts": {
        "build": "node build",
        "test": "npm run build && istanbul --config=.istanbul.yml cover _mocha -- --slow 10 --timeout 15000 --reporter spec --recursive tests",
        "test-travis": "npm run build && istanbul --config=.istanbul.yml cover _mocha -- --slow 100 --timeout 60000 --reporter spec --recursive tests",
        "test-bail": "mocha --slow 10 --timeout 15000 --reporter spec --recursive tests --bail",
        "test-only": "mocha --slow 10 --timeout 15000 --reporter spec --recursive tests",
        "test-opt": "mocha --slow 10 --timeout 15000 --reporter spec --recursive tests --bail --trace_opt --trace_deopt --trace_inlining",
        "coveralls": "cat ./testCoverage/lcov.info | ./node_modules/coveralls/bin/coveralls.js",
        "perf": "mocha --slow 60000 --timeout 60000 --reporter spec --recursive perf",
        "perf-opt": "mocha --slow 60000 --timeout 60000 --reporter spec --recursive perf --trace_opt --trace_deopt --trace_inlining",
        "prepublish": "npm run build"
    },
    "publishConfig": {
        "tag": "next"
    },
    "author": {
        "name": "Sami Koskimäki",
        "url": "https://github.com/koskimas"
    },
    "contributors": [
        "Mikael Lepistö <mikael.lepisto@vincit.com> (https://github.com/elhigu)"
    ],
    "repository": {
        "type": "git",
        "url": "git://github.com/vincit/objection.js.git"
    },
    "keywords": [
        "orm",
        "knex",
        "sql",
        "query",
        "postgresql",
        "mysql",
        "sqlite3"
    ],
    "files": [
        "README.md",
        "LICENSE",
        "lib/*",
        "src/*",
        "typings/*"
    ],
    "types": "./typings/objection/index.d.ts",
    "dependencies": {
        "ajv": "^4.11.5",
        "babel-runtime": "^6.23.0",
        "bluebird": "^3.5.0",
        "lodash": "^4.17.4"
    },
    "peerDependencies": {
        "knex": "0.x"
    },
    "devDependencies": {
        "@types/knex": "^0.0.44",
        "babel-core": "^6.24.0",
        "babel-plugin-check-es2015-constants": "^6.22.0",
        "babel-plugin-transform-class-properties": "^6.23.0",
        "babel-plugin-transform-decorators-legacy": "^1.3.4",
        "babel-plugin-transform-es2015-arrow-functions": "^6.22.0",
        "babel-plugin-transform-es2015-block-scoped-functions": "^6.22.0",
        "babel-plugin-transform-es2015-block-scoping": "^6.23.0",
        "babel-plugin-transform-es2015-classes": "^6.23.0",
        "babel-plugin-transform-es2015-computed-properties": "^6.22.0",
        "babel-plugin-transform-es2015-destructuring": "^6.23.0",
        "babel-plugin-transform-es2015-duplicate-keys": "^6.22.0",
        "babel-plugin-transform-es2015-function-name": "^6.22.0",
        "babel-plugin-transform-es2015-literals": "^6.22.0",
        "babel-plugin-transform-es2015-modules-commonjs": "^6.24.0",
        "babel-plugin-transform-es2015-parameters": "^6.23.0",
        "babel-plugin-transform-es2015-shorthand-properties": "^6.22.0",
        "babel-plugin-transform-es2015-spread": "^6.22.0",
        "babel-plugin-transform-es2015-sticky-regex": "^6.22.0",
        "babel-plugin-transform-es2015-template-literals": "^6.22.0",
        "babel-plugin-transform-es2015-typeof-symbol": "^6.23.0",
        "babel-plugin-transform-es2015-unicode-regex": "^6.22.0",
        "babel-plugin-transform-runtime": "^6.23.0",
        "coveralls": "^2.12.0",
        "expect.js": "^0.3.1",
        "fs-extra": "2.0.0",
        "glob": "^7.1.1",
        "istanbul": "^0.4.5",
        "knex": "0.x",
        "mocha": "^3.2.0",
        "mysql": "^2.13.0",
        "pg": "^6.1.5",
        "source-map-support": "^0.4.14",
        "sqlite3": "^3.1.8",
        "typescript": "^2.2.1"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
