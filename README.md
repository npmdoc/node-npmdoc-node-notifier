# npmdoc-node-notifier

#### api documentation for  [node-notifier (v5.1.2)](https://github.com/mikaelbr/node-notifier#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-node-notifier.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-node-notifier) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-notifier.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-notifier)

#### A Node.js module for sending notifications on native Mac, Windows (post and pre 8) and Linux (or Growl as fallback)

[![NPM](https://nodei.co/npm/node-notifier.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/node-notifier)

- [https://npmdoc.github.io/node-npmdoc-node-notifier/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-node-notifier/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-notifier/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-notifier/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-node-notifier/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-node-notifier/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Mikael Brevik"
    },
    "bugs": {
        "url": "https://github.com/mikaelbr/node-notifier/issues"
    },
    "dependencies": {
        "growly": "^1.3.0",
        "semver": "^5.3.0",
        "shellwords": "^0.1.0",
        "which": "^1.2.12"
    },
    "description": "A Node.js module for sending notifications on native Mac, Windows (post and pre 8) and Linux (or Growl as fallback)",
    "devDependencies": {
        "eslint": "^3.13.1",
        "eslint-config-semistandard": "^7.0.0",
        "eslint-config-standard": "^6.2.1",
        "eslint-plugin-promise": "^3.4.0",
        "eslint-plugin-standard": "^2.0.1",
        "jest": "^18.1.0"
    },
    "directories": {
        "example": "example",
        "test": "test"
    },
    "dist": {
        "shasum": "2fa9e12605fa10009d44549d6fcd8a63dde0e4ff",
        "tarball": "https://registry.npmjs.org/node-notifier/-/node-notifier-5.1.2.tgz"
    },
    "gitHead": "0b75bc5f6099bd5aeaac3e6c34e3a7e75edaba7e",
    "homepage": "https://github.com/mikaelbr/node-notifier#readme",
    "jest": {
        "testRegex": "/test/[^_]*.js",
        "testEnvironment": "node",
        "setupTestFrameworkScriptFile": "./test/_test-matchers.js"
    },
    "keywords": [
        "notification center",
        "mac os x 10.8",
        "notify",
        "terminal-notifier",
        "notify-send",
        "growl",
        "windows 8 notification",
        "toaster",
        "notification"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "mikaelb"
        }
    ],
    "name": "node-notifier",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/mikaelbr/node-notifier.git"
    },
    "scripts": {
        "example": "node ./example/message.js",
        "example:mac": "node ./example/advanced.js",
        "example:mac:input": "node ./example/macInput.js",
        "example:windows": "node ./example/toaster.js",
        "lint": "eslint example/*.js lib/*.js notifiers/*.js test/**/*.js index.js",
        "pretest": "npm run lint",
        "test": "jest"
    },
    "version": "5.1.2"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
