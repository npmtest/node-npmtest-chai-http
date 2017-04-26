# npmtest-chai-http

#### basic test coverage for  [chai-http (v3.0.0)](https://github.com/chaijs/chai-http#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-chai-http.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-chai-http) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-chai-http.svg)](https://travis-ci.org/npmtest/node-npmtest-chai-http)

#### Extend Chai Assertion library with tests for http apis

[![NPM](https://nodei.co/npm/chai-http.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/chai-http)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-chai-http/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-chai-http/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-chai-http/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-chai-http/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-chai-http/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-chai-http/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-chai-http/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-chai-http/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-chai-http/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-chai-http/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-chai-http/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-chai-http/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-chai-http/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-chai-http/build/test-report.html](https://npmtest.github.io/node-npmtest-chai-http/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-chai-http/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-chai-http/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-chai-http/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-chai-http/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-chai-http/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-chai-http/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-chai-http/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-chai-http/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jake Luer"
    },
    "browser": {
        "http": false,
        "https": false,
        "net": "./lib/net.js",
        "querystring": "qs"
    },
    "bugs": {
        "url": "https://github.com/chaijs/chai-http/issues"
    },
    "contributors": [
        {
            "name": "Jake Luer"
        },
        {
            "name": "Veselin Todorov"
        },
        {
            "name": "Keith Cirkel",
            "url": "http://keithcirkel.co.uk"
        }
    ],
    "dependencies": {
        "cookiejar": "2.0.x",
        "is-ip": "1.0.0",
        "methods": "^1.1.2",
        "qs": "^6.2.0",
        "superagent": "^2.0.0"
    },
    "description": "Extend Chai Assertion library with tests for http apis",
    "devDependencies": {
        "chai": "*",
        "coveralls": "^2.11.9",
        "dox": "^0.8.1",
        "es6-shim": "^0.35.1",
        "http-server": "^0.9.0",
        "istanbul": "^0.4.3",
        "mocha": "^2.5.3",
        "npm-run-all": "^2.1.1",
        "simplifyify": "^2.0.1"
    },
    "directories": {},
    "dist": {
        "shasum": "5460d8036e1f1a12b0b5b5cbd529e6dc1d31eb4b",
        "tarball": "https://registry.npmjs.org/chai-http/-/chai-http-3.0.0.tgz"
    },
    "engines": {
        "node": ">= 0.6.0"
    },
    "files": [
        "dist/chai-http.js",
        "lib/*.js",
        "index.js"
    ],
    "gitHead": "1345021daad2c7b0fbac9fe5c541f55802795f33",
    "homepage": "https://github.com/chaijs/chai-http#readme",
    "keywords": [
        "chai",
        "chai-plugin",
        "browser",
        "http",
        "request",
        "vendor",
        "supertest",
        "superagent"
    ],
    "main": "./index",
    "maintainers": [
        {
            "name": "chaijs"
        }
    ],
    "name": "chai-http",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/chaijs/chai-http.git"
    },
    "scripts": {
        "build": "npm run build:readme && npm run build:js",
        "build:js": "simplifyify lib/http.js --outfile dist/chai-http.js --bundle --minify --debug --standalone chaiHttp",
        "build:readme": "rm -rf README.md && node ./support/readme",
        "posttest": "if [ -z \"$COVERALLS_REPO_TOKEN\" ]; then cat coverage/lcov.info | coveralls; fi",
        "prebuild:js": "rm -rf dist",
        "server": "http-server -o -c-1",
        "start": "npm-run-all --parallel watch server",
        "test": "istanbul cover --report lcovonly _mocha",
        "watch": "npm run build:js -- --watch"
    },
    "version": "3.0.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
