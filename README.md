# api documentation for  [app-root-path (v2.0.1)](https://github.com/inxilpro/node-app-root-path)  [![npm package](https://img.shields.io/npm/v/npmdoc-app-root-path.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-app-root-path) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-app-root-path.svg)](https://travis-ci.org/npmdoc/node-npmdoc-app-root-path)
#### Determine an app's root path from anywhere inside the app

[![NPM](https://nodei.co/npm/app-root-path.png?downloads=true)](https://www.npmjs.com/package/app-root-path)

[![apidoc](https://npmdoc.github.io/node-npmdoc-app-root-path/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-app-root-path%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-app-root-path/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-app-root-path/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-app-root-path/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Chris Morrell",
        "email": "http://cmorrell.com"
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
            "name": "inxilpro",
            "email": "npm@rchy.net"
        }
    ],
    "name": "app-root-path",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module app-root-path](#apidoc.module.app-root-path)
1.  [function <span class="apidocSignatureSpan">app-root-path.</span>require (pathToModule)](#apidoc.element.app-root-path.require)
1.  [function <span class="apidocSignatureSpan">app-root-path.</span>resolve (pathToModule)](#apidoc.element.app-root-path.resolve)
1.  [function <span class="apidocSignatureSpan">app-root-path.</span>setPath (explicitlySetPath)](#apidoc.element.app-root-path.setPath)
1.  object <span class="apidocSignatureSpan">app-root-path.</span>browser_shim
1.  string <span class="apidocSignatureSpan">app-root-path.</span>path

#### [module app-root-path.browser_shim](#apidoc.module.app-root-path.browser_shim)
1.  [function <span class="apidocSignatureSpan">app-root-path.browser_shim.</span>require (pathToModule)](#apidoc.element.app-root-path.browser_shim.require)
1.  [function <span class="apidocSignatureSpan">app-root-path.browser_shim.</span>resolve (pathToModule)](#apidoc.element.app-root-path.browser_shim.resolve)
1.  [function <span class="apidocSignatureSpan">app-root-path.browser_shim.</span>setPath (explicitlySetPath)](#apidoc.element.app-root-path.browser_shim.setPath)
1.  [function <span class="apidocSignatureSpan">app-root-path.browser_shim.</span>toString ()](#apidoc.element.app-root-path.browser_shim.toString)
1.  string <span class="apidocSignatureSpan">app-root-path.browser_shim.</span>path



# <a name="apidoc.module.app-root-path"></a>[module app-root-path](#apidoc.module.app-root-path)

#### <a name="apidoc.element.app-root-path.require"></a>[function <span class="apidocSignatureSpan">app-root-path.</span>require (pathToModule)](#apidoc.element.app-root-path.require)
- description and source-code
```javascript
require = function (pathToModule) {
			return require(publicInterface.resolve(pathToModule));
		}
```
- example usage
```shell
...
  - No changes.  Just updated the version to signify a locked API (see [semver](http://semver.org/)).

### 0.1.1
  - Added Windows support (and, theoretically, other operating systems that have a directory separator that's not "/")

### 0.1.0
  - Completely rewrote the path resolution method to account for most possible scenarios.  This shouldn't cause and backwards compatibility
 issues, but always test your code.
  - Removed the need to pass a modules's 'require()' method to the 'appRootPath.require()' function.  Which it's true that each
module has its own 'require()' method, in practice it doesn't matter, and it's **much** simpler this way.
  - Added tests

## Development Nodes

When using [semantic-release](https://github.com/semantic-release/semantic-release), the preferred method
for commits is:
...
```

#### <a name="apidoc.element.app-root-path.resolve"></a>[function <span class="apidocSignatureSpan">app-root-path.</span>resolve (pathToModule)](#apidoc.element.app-root-path.resolve)
- description and source-code
```javascript
resolve = function (pathToModule) {
			return path.join(appRootPath, pathToModule);
		}
```
- example usage
```shell
...
// In lib/module/component/subcomponent.js
var myModule = reqlib('/lib/my-module.js');
'''

Finally, you can also just resolve a module path:

''' js
var myModulePath = require('app-root-path').resolve('/lib/my-module.js');
'''

You can explicitly set the path, using the environmental variable 'APP_ROOT_PATH' or by calling 'require('app-root-path').setPath
('/my/app/is/here')'

## How It Works (under the hood)

> No need to read this unless your curious—or you run into a (very unlikely) case where the module does not work as expected.
...
```

#### <a name="apidoc.element.app-root-path.setPath"></a>[function <span class="apidocSignatureSpan">app-root-path.</span>setPath (explicitlySetPath)](#apidoc.element.app-root-path.setPath)
- description and source-code
```javascript
setPath = function (explicitlySetPath) {
			appRootPath = path.resolve(explicitlySetPath);
			publicInterface.path = appRootPath;
		}
```
- example usage
```shell
...

Finally, you can also just resolve a module path:

''' js
var myModulePath = require('app-root-path').resolve('/lib/my-module.js');
'''

You can explicitly set the path, using the environmental variable 'APP_ROOT_PATH' or by calling 'require('app-root-path').setPath
('/my/app/is/here')'

## How It Works (under the hood)

> No need to read this unless your curious—or you run into a (very unlikely) case where the module does not work as expected.

This module uses two different methods to determine the app's root path, depending on the circumstances.
...
```



# <a name="apidoc.module.app-root-path.browser_shim"></a>[module app-root-path.browser_shim](#apidoc.module.app-root-path.browser_shim)

#### <a name="apidoc.element.app-root-path.browser_shim.require"></a>[function <span class="apidocSignatureSpan">app-root-path.browser_shim.</span>require (pathToModule)](#apidoc.element.app-root-path.browser_shim.require)
- description and source-code
```javascript
require = function (pathToModule) {
	return require(exports.resolve(pathToModule));
}
```
- example usage
```shell
...
  - No changes.  Just updated the version to signify a locked API (see [semver](http://semver.org/)).

### 0.1.1
  - Added Windows support (and, theoretically, other operating systems that have a directory separator that's not "/")

### 0.1.0
  - Completely rewrote the path resolution method to account for most possible scenarios.  This shouldn't cause and backwards compatibility
 issues, but always test your code.
  - Removed the need to pass a modules's 'require()' method to the 'appRootPath.require()' function.  Which it's true that each
module has its own 'require()' method, in practice it doesn't matter, and it's **much** simpler this way.
  - Added tests

## Development Nodes

When using [semantic-release](https://github.com/semantic-release/semantic-release), the preferred method
for commits is:
...
```

#### <a name="apidoc.element.app-root-path.browser_shim.resolve"></a>[function <span class="apidocSignatureSpan">app-root-path.browser_shim.</span>resolve (pathToModule)](#apidoc.element.app-root-path.browser_shim.resolve)
- description and source-code
```javascript
resolve = function (pathToModule) {
	return exports.path + pathToModule;
}
```
- example usage
```shell
...
// In lib/module/component/subcomponent.js
var myModule = reqlib('/lib/my-module.js');
'''

Finally, you can also just resolve a module path:

''' js
var myModulePath = require('app-root-path').resolve('/lib/my-module.js');
'''

You can explicitly set the path, using the environmental variable 'APP_ROOT_PATH' or by calling 'require('app-root-path').setPath
('/my/app/is/here')'

## How It Works (under the hood)

> No need to read this unless your curious—or you run into a (very unlikely) case where the module does not work as expected.
...
```

#### <a name="apidoc.element.app-root-path.browser_shim.setPath"></a>[function <span class="apidocSignatureSpan">app-root-path.browser_shim.</span>setPath (explicitlySetPath)](#apidoc.element.app-root-path.browser_shim.setPath)
- description and source-code
```javascript
setPath = function (explicitlySetPath) {
	exports.path = explicitlySetPath;
}
```
- example usage
```shell
...

Finally, you can also just resolve a module path:

''' js
var myModulePath = require('app-root-path').resolve('/lib/my-module.js');
'''

You can explicitly set the path, using the environmental variable 'APP_ROOT_PATH' or by calling 'require('app-root-path').setPath
('/my/app/is/here')'

## How It Works (under the hood)

> No need to read this unless your curious—or you run into a (very unlikely) case where the module does not work as expected.

This module uses two different methods to determine the app's root path, depending on the circumstances.
...
```

#### <a name="apidoc.element.app-root-path.browser_shim.toString"></a>[function <span class="apidocSignatureSpan">app-root-path.browser_shim.</span>toString ()](#apidoc.element.app-root-path.browser_shim.toString)
- description and source-code
```javascript
toString = function () {
	return exports.path;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
