# npmtest-node-zopfli

#### test coverage for  [node-zopfli (v2.0.2)](https://github.com/pierreinglebert/node-zopfli)  [![npm package](https://img.shields.io/npm/v/npmtest-node-zopfli.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-node-zopfli) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-node-zopfli.svg)](https://travis-ci.org/npmtest/node-npmtest-node-zopfli)

#### Bindings for Zopfli compressing lib. Compress gzip files 5% better than gzip.

[![NPM](https://nodei.co/npm/node-zopfli.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/node-zopfli)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-node-zopfli/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-node-zopfli/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-node-zopfli/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-node-zopfli/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-node-zopfli/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-node-zopfli/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-node-zopfli/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-node-zopfli/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-node-zopfli/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-node-zopfli/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-node-zopfli/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-node-zopfli/build/test-report.html](https://npmtest.github.io/node-npmtest-node-zopfli/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-node-zopfli/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-node-zopfli/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-node-zopfli/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-node-zopfli/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-zopfli/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-zopfli/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-node-zopfli/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-node-zopfli/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Pierre Inglebert"
    },
    "bin": {
        "zopfli": "bin/zopfli",
        "zopflipng": "bin/zopflipng"
    },
    "binary": {
        "module_name": "zopfli",
        "module_path": "./lib/binding/{node_abi}-{platform}-{arch}",
        "remote_path": "./{configuration}",
        "package_name": "{module_name}-v{version}-{node_abi}-{platform}-{arch}.tar.gz",
        "host": "https://node-zopfli.s3.amazonaws.com"
    },
    "bugs": {
        "url": "https://github.com/pierreinglebert/node-zopfli/issues"
    },
    "contributors": [
        {
            "name": "duralog"
        },
        {
            "name": "MayhemYDG"
        },
        {
            "name": "XhmikosR"
        }
    ],
    "dependencies": {
        "commander": "^2.8.1",
        "defaults": "^1.0.2",
        "nan": "^2.0.0",
        "node-pre-gyp": "^0.6.4"
    },
    "description": "Bindings for Zopfli compressing lib. Compress gzip files 5% better than gzip.",
    "devDependencies": {
        "async": "^2.0.0",
        "aws-sdk": "^2.4.8",
        "chai": "^3.5.0",
        "coveralls": "^2.11.2",
        "eslint": "1.0.0",
        "istanbul": "^0.4.4",
        "mocha": "^2.2.4",
        "randomstring": "^1.0.5"
    },
    "directories": {},
    "dist": {
        "shasum": "a7a473ae92aaea85d4c68d45bbf2c944c46116b8",
        "tarball": "https://registry.npmjs.org/node-zopfli/-/node-zopfli-2.0.2.tgz"
    },
    "engines": {
        "node": ">=0.12"
    },
    "files": [
        "bin",
        "lib",
        "src",
        "zopfli",
        "binding.gyp"
    ],
    "gitHead": "6adf6906ff8acbb52659b77e5f3dd445117a2287",
    "gypfile": true,
    "homepage": "https://github.com/pierreinglebert/node-zopfli",
    "keywords": [
        "zopfli",
        "zlib",
        "compress",
        "gzip",
        "deflate"
    ],
    "license": "MIT",
    "main": "lib/zopfli.js",
    "maintainers": [
        {
            "name": "pierre.inglebert"
        }
    ],
    "name": "node-zopfli",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/pierreinglebert/node-zopfli.git"
    },
    "scripts": {
        "coveralls": "coveralls < ./coverage/lcov.info",
        "install": "node-pre-gyp install --fallback-to-build",
        "lint": "eslint .",
        "mocha": "mocha test",
        "test": "npm run lint && npm run mocha",
        "test-cov": "istanbul cover ./node_modules/mocha/bin/_mocha -- -R spec test"
    },
    "version": "2.0.2"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
