# npmdoc-datapumps

#### api documentation for  [datapumps (v0.5.0)](https://github.com/agmen-hu/node-datapumps)  [![npm package](https://img.shields.io/npm/v/npmdoc-datapumps.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-datapumps) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-datapumps.svg)](https://travis-ci.org/npmdoc/node-npmdoc-datapumps)

#### Node.js ETL (Extract, Transform, Load) toolkit for easy data import, export or transfer between systems.

[![NPM](https://nodei.co/npm/datapumps.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/datapumps)

- [https://npmdoc.github.io/node-npmdoc-datapumps/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-datapumps/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-datapumps/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-datapumps/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-datapumps/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-datapumps/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Szilard Novaki",
        "url": "https://github.com/novaki"
    },
    "bugs": {
        "url": "https://github.com/agmen-hu/node-datapumps/issues"
    },
    "dependencies": {
        "bluebird": "^2.2.2",
        "coffee-script": "^1.7.1",
        "excel4node": "~0.0.9",
        "fast-csv": "~0.5.2",
        "mongodb": "^2.2.24",
        "mysql": "~2.5.1",
        "pg": "^6.1.5",
        "restler": "~3.2.2",
        "xlsx": "~0.7.8"
    },
    "description": "Node.js ETL (Extract, Transform, Load) toolkit for easy data import, export or transfer between systems.",
    "devDependencies": {
        "grunt": "~0.4.1",
        "grunt-cafe-mocha": "~0.1.12",
        "grunt-contrib-coffee": "~0.11.1",
        "grunt-contrib-watch": "~0.6.1",
        "mocha": "~1.21.3",
        "should": "~4.0.4",
        "sinon": "~1.10.3"
    },
    "directories": {},
    "dist": {
        "shasum": "f4efdaeb22a03077260abc91bdcce2a4a269231a",
        "tarball": "https://registry.npmjs.org/datapumps/-/datapumps-0.5.0.tgz"
    },
    "gitHead": "a28bd1909bac044f8f87266646c3401216be7562",
    "homepage": "https://github.com/agmen-hu/node-datapumps",
    "keywords": [
        "etl",
        "import",
        "export",
        "batch",
        "excel",
        "xlsx",
        "rest"
    ],
    "licence": "MIT",
    "maintainers": [
        {
            "name": "hendricha"
        },
        {
            "name": "neveri"
        },
        {
            "name": "novaki"
        }
    ],
    "name": "datapumps",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/agmen-hu/node-datapumps.git"
    },
    "scripts": {
        "prepublish": "coffee --no-header -o lib -c src",
        "test": "mocha --compilers coffee:coffee-script/register src/spec src/mixin/spec"
    },
    "version": "0.5.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
