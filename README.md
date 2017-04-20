# npmtest-roots

#### basic test coverage for  [roots (v5.1.0)](http://roots.cx)  [![npm package](https://img.shields.io/npm/v/npmtest-roots.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-roots) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-roots.svg)](https://travis-ci.org/npmtest/node-npmtest-roots)

#### simple, flexible, and powerful static site compiler

[![NPM](https://nodei.co/npm/roots.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/roots)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-roots/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-roots/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-roots/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-roots/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-roots/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-roots/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-roots/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-roots/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-roots/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-roots/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-roots/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-roots/build/test-report.html](https://npmtest.github.io/node-npmtest-roots/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-roots/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-roots/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-roots/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-roots/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-roots/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-roots/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-roots/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-roots/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "roots",
    "description": "simple, flexible, and powerful static site compiler",
    "version": "5.1.0",
    "author": "Jeff Escalante <hello@jenius.me>",
    "bugs": {
        "url": "https://github.com/jenius/roots/issues"
    },
    "contributors": [
        "Sam Saccone <sam@samx.it>"
    ],
    "dependencies": {
        "accord": "0.26.4",
        "argparse": "1.x",
        "browser-sync": "^2.12.5",
        "charge": "0.1.x",
        "chokidar": "^1.5.0",
        "coffee-script": "1.12.1",
        "colors": "1.x",
        "configstore": "^2.0.0",
        "graceful-fs": "^4.1.9",
        "inquirer": "^2.0.0",
        "keen.io": "0.1.x",
        "lodash": "^4.12.0",
        "micromatch": "^2.3.8",
        "mkdirp": "0.5.x",
        "npm": "^4.0.3",
        "open": "0.0.5",
        "osenv": "0.1.x",
        "readdirp": "2.x",
        "rimraf": "2.x",
        "serve-static": "1.x",
        "sprout": "^1.1.0",
        "update-notifier": "^1.0.0",
        "vinyl": "2.0.1",
        "when": "3.x"
    },
    "devDependencies": {
        "chai": "3.x",
        "chai-as-promised": "6.0.0",
        "chai-fs": "jenius/chai-fs",
        "coffeelint": "^1.15.7",
        "coveralls": "2.x",
        "glob": "^7.0.3",
        "istanbul": "^0.4.3",
        "mocha": "2.x",
        "mocha-lcov-reporter": "^1.2.0",
        "mockery": "^2.0.0",
        "roots-util": "^0.2.0",
        "sinon": "^1.17.4",
        "sinon-chai": "2.x"
    },
    "directories": {
        "lib": "lib",
        "bin": "bin"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "homepage": "http://roots.cx",
    "keywords": [
        "roots",
        "static"
    ],
    "license": "MIT",
    "main": "lib",
    "repository": {
        "type": "git",
        "url": "https://github.com/jenius/roots"
    },
    "scripts": {
        "coverage": "make build; istanbul cover _mocha --report html -- -R spec && open coverage/index.html && make unbuild",
        "coveralls": "make build; istanbul cover _mocha --report lcovonly -- -R spec && cat ./coverage/lcov.info | coveralls && rm -rf ./coverage; make unbuild",
        "lint": "coffeelint lib",
        "postinstall": "node ./post_install.js",
        "test": "npm run lint && mocha"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
