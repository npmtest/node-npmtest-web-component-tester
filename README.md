# npmtest-web-component-tester

#### basic test coverage for  [web-component-tester (v5.0.1)](https://github.com/Polymer/web-component-tester)  [![npm package](https://img.shields.io/npm/v/npmtest-web-component-tester.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-web-component-tester) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-web-component-tester.svg)](https://travis-ci.org/npmtest/node-npmtest-web-component-tester)

#### web-component-tester makes testing your web components a breeze!

[![NPM](https://nodei.co/npm/web-component-tester.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/web-component-tester)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-web-component-tester/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-web-component-tester/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-web-component-tester/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-web-component-tester/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-web-component-tester/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-web-component-tester/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-web-component-tester/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-web-component-tester/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-web-component-tester/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-web-component-tester/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-web-component-tester/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-web-component-tester/build/test-report.html](https://npmtest.github.io/node-npmtest-web-component-tester/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-web-component-tester/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-web-component-tester/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-web-component-tester/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-web-component-tester/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-web-component-tester/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-web-component-tester/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-web-component-tester/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-web-component-tester/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "web-component-tester",
    "version": "5.0.1",
    "description": "web-component-tester makes testing your web components a breeze!",
    "keywords": [
        "browser",
        "grunt",
        "gruntplugin",
        "gulp",
        "polymer",
        "test",
        "testing",
        "web component",
        "web"
    ],
    "homepage": "https://github.com/Polymer/web-component-tester",
    "bugs": "https://github.com/Polymer/web-component-tester/issues",
    "license": "BSD-3-Clause",
    "repository": {
        "type": "git",
        "url": "https://github.com/Polymer/web-component-tester.git"
    },
    "main": "runner.js",
    "bin": {
        "wct": "./bin/wct",
        "wct-st": "./bin/wct-st"
    },
    "files": [
        "bin/",
        "data/",
        "runner/",
        "scripts/",
        "tasks/",
        ".bowerrc",
        "bower.json",
        "browser.js",
        "browser.js.map",
        "package.json",
        "LICENSE",
        "README.md",
        "runner.js"
    ],
    "scripts": {
        "lint": "gulp lint",
        "build": "tsc && gulp build",
        "test": "tsc && gulp test",
        "prepublish": "gulp prepublish",
        "test:watch": "watch 'gulp test:unit' runner/ browser/ bin/ test/ tasks/",
        "format": "find runner test | grep '\\.js$\\|\\.ts$' | xargs ./node_modules/.bin/clang-format --style=file -i"
    },
    "dependencies": {
        "@types/body-parser": "0.0.33",
        "@types/chai": "^3.4.34",
        "@types/chalk": "^0.4.31",
        "@types/express": "^4.0.33",
        "@types/glob": "^5.0.30",
        "@types/grunt": "^0.4.20",
        "@types/gulp": "^3.8.32",
        "@types/lodash": "^4.14.38",
        "@types/mime": "0.0.29",
        "@types/minimatch": "^2.0.29",
        "@types/mocha": "^2.2.32",
        "@types/multer": "0.0.32",
        "@types/node": "^4.0.30",
        "@types/nomnom": "0.0.28",
        "@types/sinon": "^1.16.31",
        "@types/sinon-chai": "^2.7.27",
        "@types/socket.io": "^1.4.27",
        "accessibility-developer-tools": "^2.10.0",
        "async": "^1.5.0",
        "body-parser": "^1.14.2",
        "chai": "^3.2.0",
        "chalk": "^1.1.1",
        "cleankill": "^1.0.0",
        "express": "^4.8.5",
        "findup-sync": "^0.2.1",
        "glob": "^5.0.15",
        "lodash": "^3.0.1",
        "mocha": "^3.1.2",
        "multer": "^1.1.0",
        "nomnom": "^1.8.1",
        "promisify-node": "^0.4.0",
        "resolve": "^1.0.0",
        "send": "^0.11.1",
        "serve-waterfall": "^1.1.0",
        "server-destroy": "^1.0.1",
        "sinon": "^1.11.1",
        "sinon-chai": "^2.6.0",
        "socket.io": "^1.3.7",
        "stacky": "^1.3.1",
        "test-fixture": "PolymerElements/test-fixture",
        "wd": "^1.0.0"
    },
    "optionalDependencies": {
        "update-notifier": "^0.6.0",
        "wct-local": "^2.0.8",
        "wct-sauce": "^1.8.2"
    },
    "devDependencies": {
        "@types/express-serve-static-core": "^4.0.39",
        "bower": "^1.7.9",
        "clang-format": "^1.0.43",
        "depcheck": "^0.6.3",
        "grunt": "^0.4.5",
        "gulp": "^3.8.8",
        "gulp-bower": "0.0.13",
        "gulp-jshint": "^2.0.0",
        "gulp-spawn-mocha": "^3.1.0",
        "gulp-tslint": "^5.0.0",
        "gulp-typescript": "^3.1.2",
        "jshint": "^2.8.0",
        "jshint-stylish": "^2.0.1",
        "lazypipe": "^1.0.1",
        "rollup": "^0.25.1",
        "run-sequence": "^1.0.1",
        "tslint": "^3.10.2",
        "typescript": "^2.1.4",
        "watch": "^0.18.0"
    },
    "engines": {
        "node": ">= 4.0"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
