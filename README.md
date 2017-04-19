# npmdoc-app-root-path

#### api documentation for  [app-root-path (v2.0.1)](https://github.com/inxilpro/node-app-root-path)  [![npm package](https://img.shields.io/npm/v/npmdoc-app-root-path.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-app-root-path) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-app-root-path.svg)](https://travis-ci.org/npmdoc/node-npmdoc-app-root-path)

#### Determine an app's root path from anywhere inside the app

[![NPM](https://nodei.co/npm/app-root-path.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/app-root-path)

- [https://npmdoc.github.io/node-npmdoc-app-root-path/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-app-root-path/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-app-root-path/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-app-root-path/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-app-root-path/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-app-root-path/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Chris Morrell"
    },
    "browser": "browser-shim.js",
    "bugs": {
        "url": "https://github.com/inxilpro/node-app-root-path/issues"
    },
    "config": {
        "ghooks": {
            "commit-msg": "validate-commit-msg",
            "post-merge": "npm install",
            "post-rewrite": "npm install"
        },
        "commitizen": {
            "path": "./node_modules/cz-conventional-changelog"
        }
    },
    "dependencies": {},
    "description": "Determine an app's root path from anywhere inside the app",
    "devDependencies": {
        "codecov": "^1.0.1",
        "coveralls": "^2.11.2",
        "cracks": "^3.1.2",
        "cz-conventional-changelog": "^1.2.0",
        "ghooks": "^1.3.2",
        "istanbul": "^0.3.4",
        "mocha": "^2.0.1",
        "mocha-lcov-reporter": "0.0.1",
        "mockery": "^1.7.0",
        "nyc": "^8.1.0",
        "semantic-release": "^4.3.5",
        "validate-commit-msg": "^2.8.0"
    },
    "directories": {},
    "dist": {
        "shasum": "cd62dcf8e4fd5a417efc664d2e5b10653c651b46",
        "tarball": "https://registry.npmjs.org/app-root-path/-/app-root-path-2.0.1.tgz"
    },
    "engines": {
        "node": ">= 4.0.0"
    },
    "gitHead": "eb7e4adcf124b62564ca55d6a398073a52a97c6c",
    "homepage": "https://github.com/inxilpro/node-app-root-path",
    "keywords": [
        "root",
        "path",
        "utility",
        "util",
        "node",
        "module",
        "modules",
        "node_modules",
        "require",
        "app"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "inxilpro"
        }
    ],
    "name": "app-root-path",
    "optionalDependencies": {},
    "release": {
        "branch": "master"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/inxilpro/node-app-root-path.git"
    },
    "scripts": {
        "release": "semantic-release pre && npm publish && semantic-release post",
        "report-coverage": "npm test && nyc report --reporter=text-lcov > coverage.lcov && codecov",
        "test": "nyc mocha -R spec"
    },
    "version": "2.0.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
