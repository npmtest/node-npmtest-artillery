# npmtest-artillery

#### basic test coverage for  artillery (v1.5.8-1)  [![npm package](https://img.shields.io/npm/v/npmtest-artillery.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-artillery) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-artillery.svg)](https://travis-ci.org/npmtest/node-npmtest-artillery)

#### Load-testing for HTTP and WebSocket-based applications

[![NPM](https://nodei.co/npm/artillery.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/artillery)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-artillery/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-artillery/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-artillery/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-artillery/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-artillery/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-artillery/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-artillery/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-artillery/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-artillery/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-artillery/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-artillery/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-artillery/build/test-report.html](https://npmtest.github.io/node-npmtest-artillery/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-artillery/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-artillery/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-artillery/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-artillery/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-artillery/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-artillery/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-artillery/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-artillery/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "artillery",
    "version": "1.5.8-1",
    "description": "Load-testing for HTTP and WebSocket-based applications",
    "main": "./lib",
    "engines": {
        "node": ">= 4.2.0"
    },
    "scripts": {
        "test": "bash test/runner.sh",
        "is_formatted": "find . -name '*.js' | grep -v node_modules | grep -v coverage | xargs jscs --preset=google",
        "is_linted": "find . -name '*.js' | grep -v node_modules | grep -v coverage | xargs eslint",
        "coverage": "npm_config_coverage=y npm test && istanbul report html text-summary"
    },
    "keywords": [
        "load testing",
        "stress testing",
        "benchmark",
        "performance",
        "blackbox testing"
    ],
    "author": "Hassy Veldstra <h@veldstra.org>",
    "contributors": [
        "Kieran Gorman (https://github.com/kjgorman)",
        "Antony Jones (https://github.com/antony)"
    ],
    "license": "MPL-2.0",
    "preferGlobal": true,
    "man": "./man/artillery.1",
    "bin": {
        "artillery": "./bin/artillery"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/shoreditch-ops/artillery.git"
    },
    "bugs": {
        "url": "https://github.com/shoreditch-ops/artillery/issues"
    },
    "dependencies": {
        "arrivals": "^2.0.2",
        "artillery-core": "4.0.3",
        "async": "^1.0.0",
        "chalk": "1.1.3",
        "cli": "^0.6.6",
        "commander": "2.9.0",
        "csv-parse": "^0.1.1",
        "debug": "2.2.0",
        "lodash": "4.17.2",
        "moment": "2.11.2",
        "open": "0.0.5",
        "rc": "^1.1.6",
        "tmp": "0.0.28",
        "yaml-js": "0.1.4"
    },
    "devDependencies": {
        "bats": "^0.4.2",
        "eslint": "^0.21.2",
        "good": "^6.4.0",
        "good-console": "^5.2.0",
        "hapi": "^12.1.0",
        "istanbul": "^0.3.14",
        "jscs": "^2.3.0",
        "pre-commit": "^1.0.7",
        "tape": "^4.0.0",
        "uuid": "^2.0.1"
    },
    "pre-commit": [
        "is_linted"
    ]
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
