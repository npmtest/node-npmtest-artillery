# npmtest-artillery

#### basic test coverage for  [artillery (v1.5.6)](https://github.com/shoreditch-ops/artillery#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-artillery.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-artillery) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-artillery.svg)](https://travis-ci.org/npmtest/node-npmtest-artillery)

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
    "author": {
        "name": "Hassy Veldstra"
    },
    "bin": {
        "artillery": "./bin/artillery"
    },
    "bugs": {
        "url": "https://github.com/shoreditch-ops/artillery/issues"
    },
    "contributors": [
        {
            "name": "Kieran Gorman",
            "url": "https://github.com/kjgorman"
        },
        {
            "name": "Antony Jones",
            "url": "https://github.com/antony"
        }
    ],
    "dependencies": {
        "arrivals": "^2.0.2",
        "artillery-core": "3.0.0",
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
    "description": "Load-testing for HTTP and WebSocket-based applications",
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
    "directories": {},
    "dist": {
        "shasum": "6ffbff07b3071d7f653e421be10c4e389e51895a",
        "tarball": "https://registry.npmjs.org/artillery/-/artillery-1.5.6.tgz"
    },
    "engines": {
        "node": ">= 4.2.0"
    },
    "gitHead": "37d4e7c076e6171ae478b88531903fc12efb5d66",
    "homepage": "https://github.com/shoreditch-ops/artillery#readme",
    "keywords": [
        "load testing",
        "stress testing",
        "benchmark",
        "performance",
        "blackbox testing"
    ],
    "license": "MPL-2.0",
    "main": "./lib",
    "maintainers": [
        {
            "name": "hhvhhv"
        }
    ],
    "man": [
        "./man/artillery.1"
    ],
    "name": "artillery",
    "optionalDependencies": {},
    "pre-commit": [
        "is_linted"
    ],
    "preferGlobal": true,
    "repository": {
        "type": "git",
        "url": "git+https://github.com/shoreditch-ops/artillery.git"
    },
    "scripts": {
        "coverage": "npm_config_coverage=y npm test && istanbul report html text-summary",
        "is_formatted": "find . -name '*.js' | grep -v node_modules | grep -v coverage | xargs jscs --preset=google",
        "is_linted": "find . -name '*.js' | grep -v node_modules | grep -v coverage | xargs eslint",
        "test": "bash test/runner.sh"
    },
    "version": "1.5.6"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
