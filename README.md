# api documentation for  [datapumps (v0.5.0)](https://github.com/agmen-hu/node-datapumps)  [![npm package](https://img.shields.io/npm/v/npmdoc-datapumps.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-datapumps) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-datapumps.svg)](https://travis-ci.org/npmdoc/node-npmdoc-datapumps)
#### Node.js ETL (Extract, Transform, Load) toolkit for easy data import, export or transfer between systems.

[![NPM](https://nodei.co/npm/datapumps.png?downloads=true)](https://www.npmjs.com/package/datapumps)

[![apidoc](https://npmdoc.github.io/node-npmdoc-datapumps/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-datapumps_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-datapumps/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-datapumps/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-datapumps/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Szilard Novaki",
        "email": "novaki@agmen.hu",
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
            "name": "hendricha",
            "email": "hendricha@agmen.hu"
        },
        {
            "name": "neveri",
            "email": "nevi@agmen.hu"
        },
        {
            "name": "novaki",
            "email": "novaki@agmen.hu"
        }
    ],
    "name": "datapumps",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module datapumps](#apidoc.module.datapumps)
1.  [function <span class="apidocSignatureSpan">datapumps.</span>Buffer (options)](#apidoc.element.datapumps.Buffer)
1.  [function <span class="apidocSignatureSpan">datapumps.</span>Group ()](#apidoc.element.datapumps.Group)
1.  [function <span class="apidocSignatureSpan">datapumps.</span>Pump ()](#apidoc.element.datapumps.Pump)
1.  [function <span class="apidocSignatureSpan">datapumps.</span>PumpingFailedError (message)](#apidoc.element.datapumps.PumpingFailedError)
1.  [function <span class="apidocSignatureSpan">datapumps.</span>group ()](#apidoc.element.datapumps.group)
1.  object <span class="apidocSignatureSpan">datapumps.</span>Buffer.prototype
1.  object <span class="apidocSignatureSpan">datapumps.</span>Group.prototype
1.  object <span class="apidocSignatureSpan">datapumps.</span>Pump.prototype
1.  object <span class="apidocSignatureSpan">datapumps.</span>PumpingFailedError.prototype
1.  object <span class="apidocSignatureSpan">datapumps.</span>mixin

#### [module datapumps.Buffer](#apidoc.module.datapumps.Buffer)
1.  boolean <span class="apidocSignatureSpan">datapumps.Buffer.</span>usingDomains
1.  [function <span class="apidocSignatureSpan">datapumps.</span>Buffer (options)](#apidoc.element.datapumps.Buffer.Buffer)
1.  [function <span class="apidocSignatureSpan">datapumps.Buffer.</span>EventEmitter ()](#apidoc.element.datapumps.Buffer.EventEmitter)
1.  [function <span class="apidocSignatureSpan">datapumps.Buffer.</span>defaultBufferSize (size)](#apidoc.element.datapumps.Buffer.defaultBufferSize)
1.  [function <span class="apidocSignatureSpan">datapumps.Buffer.</span>init ()](#apidoc.element.datapumps.Buffer.init)
1.  [function <span class="apidocSignatureSpan">datapumps.Buffer.</span>listenerCount (emitter, type)](#apidoc.element.datapumps.Buffer.listenerCount)
1.  number <span class="apidocSignatureSpan">datapumps.Buffer.</span>_defaultBufferSize
1.  number <span class="apidocSignatureSpan">datapumps.Buffer.</span>defaultMaxListeners
1.  object <span class="apidocSignatureSpan">datapumps.Buffer.</span>__super__

#### [module datapumps.Buffer.prototype](#apidoc.module.datapumps.Buffer.prototype)
1.  [function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>_writeArrayItem (dataArray, pendingPromise, index)](#apidoc.element.datapumps.Buffer.prototype._writeArrayItem)
1.  [function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>append (data)](#apidoc.element.datapumps.Buffer.prototype.append)
1.  [function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>appendArray (dataArray)](#apidoc.element.datapumps.Buffer.prototype.appendArray)
1.  [function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>constructor (options)](#apidoc.element.datapumps.Buffer.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>getContent ()](#apidoc.element.datapumps.Buffer.prototype.getContent)
1.  [function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>isEmpty ()](#apidoc.element.datapumps.Buffer.prototype.isEmpty)
1.  [function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>isEnded ()](#apidoc.element.datapumps.Buffer.prototype.isEnded)
1.  [function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>isFull ()](#apidoc.element.datapumps.Buffer.prototype.isFull)
1.  [function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>isSealed ()](#apidoc.element.datapumps.Buffer.prototype.isSealed)
1.  [function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>read ()](#apidoc.element.datapumps.Buffer.prototype.read)
1.  [function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>readAsync ()](#apidoc.element.datapumps.Buffer.prototype.readAsync)
1.  [function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>seal ()](#apidoc.element.datapumps.Buffer.prototype.seal)
1.  [function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>write (data)](#apidoc.element.datapumps.Buffer.prototype.write)
1.  [function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>writeArrayAsync (dataArray)](#apidoc.element.datapumps.Buffer.prototype.writeArrayAsync)
1.  [function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>writeAsync (data)](#apidoc.element.datapumps.Buffer.prototype.writeAsync)

#### [module datapumps.Group](#apidoc.module.datapumps.Group)
1.  boolean <span class="apidocSignatureSpan">datapumps.Group.</span>usingDomains
1.  [function <span class="apidocSignatureSpan">datapumps.</span>Group ()](#apidoc.element.datapumps.Group.Group)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.</span>EventEmitter ()](#apidoc.element.datapumps.Group.EventEmitter)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.</span>init ()](#apidoc.element.datapumps.Group.init)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.</span>listenerCount (emitter, type)](#apidoc.element.datapumps.Group.listenerCount)
1.  number <span class="apidocSignatureSpan">datapumps.Group.</span>ABORTED
1.  number <span class="apidocSignatureSpan">datapumps.Group.</span>ENDED
1.  number <span class="apidocSignatureSpan">datapumps.Group.</span>PAUSED
1.  number <span class="apidocSignatureSpan">datapumps.Group.</span>STARTED
1.  number <span class="apidocSignatureSpan">datapumps.Group.</span>STOPPED
1.  number <span class="apidocSignatureSpan">datapumps.Group.</span>defaultMaxListeners
1.  object <span class="apidocSignatureSpan">datapumps.Group.</span>__super__

#### [module datapumps.Group.prototype](#apidoc.module.datapumps.Group.prototype)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>_endGroup ()](#apidoc.element.datapumps.Group.prototype._endGroup)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>_getAllStoppedPumps ()](#apidoc.element.datapumps.Group.prototype._getAllStoppedPumps)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>_getBufferByPath (bufferPath)](#apidoc.element.datapumps.Group.prototype._getBufferByPath)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>abort ()](#apidoc.element.datapumps.Group.prototype.abort)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>addInputPump (name, pump)](#apidoc.element.datapumps.Group.prototype.addInputPump)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>addPump (name, pump)](#apidoc.element.datapumps.Group.prototype.addPump)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>buffer (name)](#apidoc.element.datapumps.Group.prototype.buffer)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>constructor ()](#apidoc.element.datapumps.Group.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>debugMode (_debug)](#apidoc.element.datapumps.Group.prototype.debugMode)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>expose (exposedName, bufferPath)](#apidoc.element.datapumps.Group.prototype.expose)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>from (buffer)](#apidoc.element.datapumps.Group.prototype.from)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>id (id)](#apidoc.element.datapumps.Group.prototype.id)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>inputPump (pumpName)](#apidoc.element.datapumps.Group.prototype.inputPump)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>mixin (mixins)](#apidoc.element.datapumps.Group.prototype.mixin)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>pause ()](#apidoc.element.datapumps.Group.prototype.pause)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>process ()](#apidoc.element.datapumps.Group.prototype.process)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>pump (name)](#apidoc.element.datapumps.Group.prototype.pump)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>pumps ()](#apidoc.element.datapumps.Group.prototype.pumps)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>resume ()](#apidoc.element.datapumps.Group.prototype.resume)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>run ()](#apidoc.element.datapumps.Group.prototype.run)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>runPumps (pumps)](#apidoc.element.datapumps.Group.prototype.runPumps)
1.  [function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>start ()](#apidoc.element.datapumps.Group.prototype.start)

#### [module datapumps.Pump](#apidoc.module.datapumps.Pump)
1.  boolean <span class="apidocSignatureSpan">datapumps.Pump.</span>usingDomains
1.  [function <span class="apidocSignatureSpan">datapumps.</span>Pump ()](#apidoc.element.datapumps.Pump.Pump)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.</span>EventEmitter ()](#apidoc.element.datapumps.Pump.EventEmitter)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.</span>init ()](#apidoc.element.datapumps.Pump.init)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.</span>listenerCount (emitter, type)](#apidoc.element.datapumps.Pump.listenerCount)
1.  number <span class="apidocSignatureSpan">datapumps.Pump.</span>ABORTED
1.  number <span class="apidocSignatureSpan">datapumps.Pump.</span>ENDED
1.  number <span class="apidocSignatureSpan">datapumps.Pump.</span>PAUSED
1.  number <span class="apidocSignatureSpan">datapumps.Pump.</span>STARTED
1.  number <span class="apidocSignatureSpan">datapumps.Pump.</span>STOPPED
1.  number <span class="apidocSignatureSpan">datapumps.Pump.</span>defaultMaxListeners
1.  object <span class="apidocSignatureSpan">datapumps.Pump.</span>__super__

#### [module datapumps.Pump.prototype](#apidoc.module.datapumps.Pump.prototype)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>_outputBufferEnded ()](#apidoc.element.datapumps.Pump.prototype._outputBufferEnded)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>_process (data)](#apidoc.element.datapumps.Pump.prototype._process)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>_pump ()](#apidoc.element.datapumps.Pump.prototype._pump)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>_registerErrorBufferEvents ()](#apidoc.element.datapumps.Pump.prototype._registerErrorBufferEvents)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>abort ()](#apidoc.element.datapumps.Pump.prototype.abort)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>buffer (name, buffer)](#apidoc.element.datapumps.Pump.prototype.buffer)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>buffers (buffers)](#apidoc.element.datapumps.Pump.prototype.buffers)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>constructor ()](#apidoc.element.datapumps.Pump.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>copy (data, buffers)](#apidoc.element.datapumps.Pump.prototype.copy)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>createBuffer (options)](#apidoc.element.datapumps.Pump.prototype.createBuffer)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>debug ()](#apidoc.element.datapumps.Pump.prototype.debug)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>debugMode (_debug)](#apidoc.element.datapumps.Pump.prototype.debugMode)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>errorBuffer (buffer)](#apidoc.element.datapumps.Pump.prototype.errorBuffer)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>from (buffer)](#apidoc.element.datapumps.Pump.prototype.from)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>id (id)](#apidoc.element.datapumps.Pump.prototype.id)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>isEnded ()](#apidoc.element.datapumps.Pump.prototype.isEnded)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>isPaused ()](#apidoc.element.datapumps.Pump.prototype.isPaused)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>isStarted ()](#apidoc.element.datapumps.Pump.prototype.isStarted)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>isStopped ()](#apidoc.element.datapumps.Pump.prototype.isStopped)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>logErrorsToConsole ()](#apidoc.element.datapumps.Pump.prototype.logErrorsToConsole)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>mixin (mixins)](#apidoc.element.datapumps.Pump.prototype.mixin)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>pause ()](#apidoc.element.datapumps.Pump.prototype.pause)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>process (fn)](#apidoc.element.datapumps.Pump.prototype.process)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>resume ()](#apidoc.element.datapumps.Pump.prototype.resume)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>run ()](#apidoc.element.datapumps.Pump.prototype.run)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>sealOutputBuffers ()](#apidoc.element.datapumps.Pump.prototype.sealOutputBuffers)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>sourceEnded ()](#apidoc.element.datapumps.Pump.prototype.sourceEnded)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>start ()](#apidoc.element.datapumps.Pump.prototype.start)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>to (pump, bufferName)](#apidoc.element.datapumps.Pump.prototype.to)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>whenFinished ()](#apidoc.element.datapumps.Pump.prototype.whenFinished)
1.  [function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>writeError (err)](#apidoc.element.datapumps.Pump.prototype.writeError)

#### [module datapumps.PumpingFailedError](#apidoc.module.datapumps.PumpingFailedError)
1.  [function <span class="apidocSignatureSpan">datapumps.</span>PumpingFailedError (message)](#apidoc.element.datapumps.PumpingFailedError.PumpingFailedError)
1.  [function <span class="apidocSignatureSpan">datapumps.PumpingFailedError.</span>captureStackTrace ()](#apidoc.element.datapumps.PumpingFailedError.captureStackTrace)
1.  number <span class="apidocSignatureSpan">datapumps.PumpingFailedError.</span>stackTraceLimit
1.  object <span class="apidocSignatureSpan">datapumps.PumpingFailedError.</span>__super__

#### [module datapumps.PumpingFailedError.prototype](#apidoc.module.datapumps.PumpingFailedError.prototype)
1.  [function <span class="apidocSignatureSpan">datapumps.PumpingFailedError.prototype.</span>constructor (message)](#apidoc.element.datapumps.PumpingFailedError.prototype.constructor)
1.  string <span class="apidocSignatureSpan">datapumps.PumpingFailedError.prototype.</span>name

#### [module datapumps.mixin](#apidoc.module.datapumps.mixin)
1.  [function <span class="apidocSignatureSpan">datapumps.mixin.</span>BatchMixin (target)](#apidoc.element.datapumps.mixin.BatchMixin)
1.  [function <span class="apidocSignatureSpan">datapumps.mixin.</span>BufferDebugMixin (pump)](#apidoc.element.datapumps.mixin.BufferDebugMixin)
1.  [function <span class="apidocSignatureSpan">datapumps.mixin.</span>CsvWriterMixin (options)](#apidoc.element.datapumps.mixin.CsvWriterMixin)
1.  [function <span class="apidocSignatureSpan">datapumps.mixin.</span>ExcelReaderMixin (_arg)](#apidoc.element.datapumps.mixin.ExcelReaderMixin)
1.  [function <span class="apidocSignatureSpan">datapumps.mixin.</span>ExcelWriterMixin (onMixin)](#apidoc.element.datapumps.mixin.ExcelWriterMixin)
1.  [function <span class="apidocSignatureSpan">datapumps.mixin.</span>MergeMixin (pump)](#apidoc.element.datapumps.mixin.MergeMixin)
1.  [function <span class="apidocSignatureSpan">datapumps.mixin.</span>MongodbMixin (db)](#apidoc.element.datapumps.mixin.MongodbMixin)
1.  [function <span class="apidocSignatureSpan">datapumps.mixin.</span>MysqlMixin (connection)](#apidoc.element.datapumps.mixin.MysqlMixin)
1.  [function <span class="apidocSignatureSpan">datapumps.mixin.</span>ObjectTransformMixin ()](#apidoc.element.datapumps.mixin.ObjectTransformMixin)
1.  [function <span class="apidocSignatureSpan">datapumps.mixin.</span>RestMixin (target)](#apidoc.element.datapumps.mixin.RestMixin)



# <a name="apidoc.module.datapumps"></a>[module datapumps](#apidoc.module.datapumps)

#### <a name="apidoc.element.datapumps.Buffer"></a>[function <span class="apidocSignatureSpan">datapumps.</span>Buffer (options)](#apidoc.element.datapumps.Buffer)
- description and source-code
```javascript
function Buffer(options) {
  var _ref, _ref1, _ref2;
  if (options == null) {
    options = {};
  }
  this.content = (_ref = options.content) != null ? _ref : [];
  this.size = (_ref1 = options.size) != null ? _ref1 : Buffer._defaultBufferSize;
  this._sealed = (_ref2 = options.sealed) != null ? _ref2 : false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Group"></a>[function <span class="apidocSignatureSpan">datapumps.</span>Group ()](#apidoc.element.datapumps.Group)
- description and source-code
```javascript
function Group() {
  Group.__super__.constructor.call(this);
  this._pumps = {};
  this._exposedBuffers = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump"></a>[function <span class="apidocSignatureSpan">datapumps.</span>Pump ()](#apidoc.element.datapumps.Pump)
- description and source-code
```javascript
function Pump() {
  this._state = Pump.STOPPED;
  this._from = null;
  this._id = null;
  this._errorBuffer = new Buffer;
  this._debug = false;
  this.buffers({
    output: new Buffer
  });
}
```
- example usage
```shell
...
   The '.logErrorsToConsole()' will log any error to the console, surprisingly. The pump will start
   on calling '.run()'. It returns a [promise](https://promisesaplus.com/) that resolves when the pump finished.

## Pump
A pump reads data from its input buffer or stream and copies it to the output buffer by default:
'''js
datapumps = require('datapumps');
(pump = new datapumps.Pump())
  .from(<put a nodejs stream or datapumps buffer here>)
  .run()
'''

To access the output buffer, use the '.buffer()' method, which returns a Buffer instance:
'''js
buffer = pump.buffer('output');
...
```

#### <a name="apidoc.element.datapumps.PumpingFailedError"></a>[function <span class="apidocSignatureSpan">datapumps.</span>PumpingFailedError (message)](#apidoc.element.datapumps.PumpingFailedError)
- description and source-code
```javascript
function PumpingFailedError(message) {
  this.message = message != null ? message : 'Pumping failed. See .errorBuffer() contents for error messages';
  PumpingFailedError.__super__.constructor.call(this, this.message);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.group"></a>[function <span class="apidocSignatureSpan">datapumps.</span>group ()](#apidoc.element.datapumps.group)
- description and source-code
```javascript
group = function () { return new Group(); }
```
- example usage
```shell
...
})
'''

## Pump group
You often need multiple pumps to complete an ETL task. Pump groups help starting multiple pump in
one step, and also enables handling the event when every pump ended:
'''js
sendMails = datapumps.group();
sendMails.addPump('tickets')
...;
sendMails.addPump('reminderMailer')
...;
sendMails
.start()
.whenFinished().then(function() {
...
```



# <a name="apidoc.module.datapumps.Buffer"></a>[module datapumps.Buffer](#apidoc.module.datapumps.Buffer)

#### <a name="apidoc.element.datapumps.Buffer.Buffer"></a>[function <span class="apidocSignatureSpan">datapumps.</span>Buffer (options)](#apidoc.element.datapumps.Buffer.Buffer)
- description and source-code
```javascript
function Buffer(options) {
  var _ref, _ref1, _ref2;
  if (options == null) {
    options = {};
  }
  this.content = (_ref = options.content) != null ? _ref : [];
  this.size = (_ref1 = options.size) != null ? _ref1 : Buffer._defaultBufferSize;
  this._sealed = (_ref2 = options.sealed) != null ? _ref2 : false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Buffer.EventEmitter"></a>[function <span class="apidocSignatureSpan">datapumps.Buffer.</span>EventEmitter ()](#apidoc.element.datapumps.Buffer.EventEmitter)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Buffer.defaultBufferSize"></a>[function <span class="apidocSignatureSpan">datapumps.Buffer.</span>defaultBufferSize (size)](#apidoc.element.datapumps.Buffer.defaultBufferSize)
- description and source-code
```javascript
defaultBufferSize = function (size) {
  if (size == null) {
    return Buffer._defaultBufferSize;
  }
  return Buffer._defaultBufferSize = size;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Buffer.init"></a>[function <span class="apidocSignatureSpan">datapumps.Buffer.</span>init ()](#apidoc.element.datapumps.Buffer.init)
- description and source-code
```javascript
init = function () {
  this.domain = null;
  if (EventEmitter.usingDomains) {
    // if there is an active domain, then attach to it.
    domain = domain || require('domain');
    if (domain.active && !(this instanceof domain.Domain)) {
      this.domain = domain.active;
    }
  }

  if (!this._events || this._events === Object.getPrototypeOf(this)._events) {
    this._events = new EventHandlers();
    this._eventsCount = 0;
  }

  this._maxListeners = this._maxListeners || undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Buffer.listenerCount"></a>[function <span class="apidocSignatureSpan">datapumps.Buffer.</span>listenerCount (emitter, type)](#apidoc.element.datapumps.Buffer.listenerCount)
- description and source-code
```javascript
listenerCount = function (emitter, type) {
  if (typeof emitter.listenerCount === 'function') {
    return emitter.listenerCount(type);
  } else {
    return listenerCount.call(emitter, type);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.datapumps.Buffer.prototype"></a>[module datapumps.Buffer.prototype](#apidoc.module.datapumps.Buffer.prototype)

#### <a name="apidoc.element.datapumps.Buffer.prototype._writeArrayItem"></a>[function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>_writeArrayItem (dataArray, pendingPromise, index)](#apidoc.element.datapumps.Buffer.prototype._writeArrayItem)
- description and source-code
```javascript
_writeArrayItem = function (dataArray, pendingPromise, index) {
  return this.writeAsync(dataArray[index]).done((function(_this) {
    return function() {
      if (index >= dataArray.length - 1) {
        return pendingPromise.resolve();
      }
      return _this._writeArrayItem(dataArray, pendingPromise, index + 1);
    };
  })(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Buffer.prototype.append"></a>[function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>append (data)](#apidoc.element.datapumps.Buffer.prototype.append)
- description and source-code
```javascript
append = function (data) {
  this.appendArray([data]);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Buffer.prototype.appendArray"></a>[function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>appendArray (dataArray)](#apidoc.element.datapumps.Buffer.prototype.appendArray)
- description and source-code
```javascript
appendArray = function (dataArray) {
  var data, newSize, _i, _len;
  newSize = this.content.length + dataArray.length;
  if (newSize > this.size) {
    this.size = newSize;
  }
  for (_i = 0, _len = dataArray.length; _i < _len; _i++) {
    data = dataArray[_i];
    this.write(data);
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Buffer.prototype.constructor"></a>[function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>constructor (options)](#apidoc.element.datapumps.Buffer.prototype.constructor)
- description and source-code
```javascript
function Buffer(options) {
  var _ref, _ref1, _ref2;
  if (options == null) {
    options = {};
  }
  this.content = (_ref = options.content) != null ? _ref : [];
  this.size = (_ref1 = options.size) != null ? _ref1 : Buffer._defaultBufferSize;
  this._sealed = (_ref2 = options.sealed) != null ? _ref2 : false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Buffer.prototype.getContent"></a>[function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>getContent ()](#apidoc.element.datapumps.Buffer.prototype.getContent)
- description and source-code
```javascript
getContent = function () {
  return this.content;
}
```
- example usage
```shell
...
'''js
group
  .start()
  .whenFinished()
    .then(function() {
      if (!group.errorBuffer().isEmpty()) {
        console.log("Transfer finished, but with errors.");
        // errors list will be at group.errorBuffer().getContent()
      }
    })
    .catch(function() {
      console.log("Pump group failed with errors");
      // errors list will be at group.errorBuffer().getContent()
    });
'''
...
```

#### <a name="apidoc.element.datapumps.Buffer.prototype.isEmpty"></a>[function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>isEmpty ()](#apidoc.element.datapumps.Buffer.prototype.isEmpty)
- description and source-code
```javascript
isEmpty = function () {
  return this.content.length === 0;
}
```
- example usage
```shell
...
the pump group has an error buffer ('.errorBuffer()') which can hold ten error messages by default.
When the error buffer fills up, 'error' event is triggered and '.whenFinised()' promise is rejected:
'''js
group
.start()
.whenFinished()
  .then(function() {
    if (!group.errorBuffer().isEmpty()) {
      console.log("Transfer finished, but with errors.");
      // errors list will be at group.errorBuffer().getContent()
    }
  })
  .catch(function() {
    console.log("Pump group failed with errors");
    // errors list will be at group.errorBuffer().getContent()
...
```

#### <a name="apidoc.element.datapumps.Buffer.prototype.isEnded"></a>[function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>isEnded ()](#apidoc.element.datapumps.Buffer.prototype.isEnded)
- description and source-code
```javascript
isEnded = function () {
  return this.isSealed() && this.isEmpty();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Buffer.prototype.isFull"></a>[function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>isFull ()](#apidoc.element.datapumps.Buffer.prototype.isFull)
- description and source-code
```javascript
isFull = function () {
  return this.content.length >= this.size;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Buffer.prototype.isSealed"></a>[function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>isSealed ()](#apidoc.element.datapumps.Buffer.prototype.isSealed)
- description and source-code
```javascript
isSealed = function () {
  return this._sealed === true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Buffer.prototype.read"></a>[function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>read ()](#apidoc.element.datapumps.Buffer.prototype.read)
- description and source-code
```javascript
read = function () {
  var result;
  if (this.isEmpty()) {
    throw new Error('Buffer is empty');
  }
  result = this.content.shift();
  this.emit('release', result);
  if (this.isEmpty()) {
    this.emit('empty');
    if (this._sealed === true) {
      this.emit('end');
    }
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Buffer.prototype.readAsync"></a>[function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>readAsync ()](#apidoc.element.datapumps.Buffer.prototype.readAsync)
- description and source-code
```javascript
readAsync = function () {
  if (!this.isEmpty()) {
    return Promise.resolve(this.read());
  } else {
    return new Promise((function(_this) {
      return function(resolve, reject) {
        return _this.once('write', function() {
          return resolve(_this.readAsync());
        });
      };
    })(this));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Buffer.prototype.seal"></a>[function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>seal ()](#apidoc.element.datapumps.Buffer.prototype.seal)
- description and source-code
```javascript
seal = function () {
  if (this._sealed === true) {
    throw new Error('Buffer already sealed');
  }
  this._sealed = true;
  this.emit('sealed');
  if (this.isEmpty()) {
    this.emit('end');
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Buffer.prototype.write"></a>[function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>write (data)](#apidoc.element.datapumps.Buffer.prototype.write)
- description and source-code
```javascript
write = function (data) {
  if (this._sealed === true) {
    throw new Error('Cannot write sealed buffer');
  }
  if (this.isFull()) {
    throw new Error('Buffer is full');
  }
  this.content.push(data);
  this.emit('write', data);
  if (this.isFull()) {
    this.emit('full');
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Buffer.prototype.writeArrayAsync"></a>[function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>writeArrayAsync (dataArray)](#apidoc.element.datapumps.Buffer.prototype.writeArrayAsync)
- description and source-code
```javascript
writeArrayAsync = function (dataArray) {
  var result;
  if (dataArray.length === 0) {
    return Promise.resolve();
  }
  result = Promise.pending();
  this._writeArrayItem(dataArray, result, 0);
  return result.promise;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Buffer.prototype.writeAsync"></a>[function <span class="apidocSignatureSpan">datapumps.Buffer.prototype.</span>writeAsync (data)](#apidoc.element.datapumps.Buffer.prototype.writeAsync)
- description and source-code
```javascript
writeAsync = function (data) {
  if (!this.isFull()) {
    return Promise.resolve(this.write(data));
  } else {
    return new Promise((function(_this) {
      return function(resolve, reject) {
        return _this.once('release', function() {
          return resolve(_this.writeAsync(data));
        });
      };
    })(this));
  }
}
```
- example usage
```shell
...

### Transforming data
Use the '.process()' method to set the function which processes data:
'''js
ticketsPump
  .process(function(ticket) {
    ticket.title = 'URGENT: ' + ticket.title;
    return this.buffer('openTickets').writeAsync(ticket);
  });
'''
The argument of '.process()' is a function that will be executed after the pump reads a data item.
The function is executed in the context of the pump object, i.e. 'this' refers to the pump itself. The
function should return a Promise that fulfills when the data is processed (i.e. written into a buffer
or stored elsewhere).
...
```



# <a name="apidoc.module.datapumps.Group"></a>[module datapumps.Group](#apidoc.module.datapumps.Group)

#### <a name="apidoc.element.datapumps.Group.Group"></a>[function <span class="apidocSignatureSpan">datapumps.</span>Group ()](#apidoc.element.datapumps.Group.Group)
- description and source-code
```javascript
function Group() {
  Group.__super__.constructor.call(this);
  this._pumps = {};
  this._exposedBuffers = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Group.EventEmitter"></a>[function <span class="apidocSignatureSpan">datapumps.Group.</span>EventEmitter ()](#apidoc.element.datapumps.Group.EventEmitter)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Group.init"></a>[function <span class="apidocSignatureSpan">datapumps.Group.</span>init ()](#apidoc.element.datapumps.Group.init)
- description and source-code
```javascript
init = function () {
  this.domain = null;
  if (EventEmitter.usingDomains) {
    // if there is an active domain, then attach to it.
    domain = domain || require('domain');
    if (domain.active && !(this instanceof domain.Domain)) {
      this.domain = domain.active;
    }
  }

  if (!this._events || this._events === Object.getPrototypeOf(this)._events) {
    this._events = new EventHandlers();
    this._eventsCount = 0;
  }

  this._maxListeners = this._maxListeners || undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Group.listenerCount"></a>[function <span class="apidocSignatureSpan">datapumps.Group.</span>listenerCount (emitter, type)](#apidoc.element.datapumps.Group.listenerCount)
- description and source-code
```javascript
listenerCount = function (emitter, type) {
  if (typeof emitter.listenerCount === 'function') {
    return emitter.listenerCount(type);
  } else {
    return listenerCount.call(emitter, type);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.datapumps.Group.prototype"></a>[module datapumps.Group.prototype](#apidoc.module.datapumps.Group.prototype)

#### <a name="apidoc.element.datapumps.Group.prototype._endGroup"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>_endGroup ()](#apidoc.element.datapumps.Group.prototype._endGroup)
- description and source-code
```javascript
_endGroup = function () {
  this._state = Group.ENDED;
  return this.emit('end');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Group.prototype._getAllStoppedPumps"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>_getAllStoppedPumps ()](#apidoc.element.datapumps.Group.prototype._getAllStoppedPumps)
- description and source-code
```javascript
_getAllStoppedPumps = function () {
  var name, pump, result, _ref;
  result = [];
  _ref = this._pumps;
  for (name in _ref) {
    pump = _ref[name];
    if (pump.isStopped()) {
      result.push(name);
    }
  }
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Group.prototype._getBufferByPath"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>_getBufferByPath (bufferPath)](#apidoc.element.datapumps.Group.prototype._getBufferByPath)
- description and source-code
```javascript
_getBufferByPath = function (bufferPath) {
  var bufferName, bufferNames, pumpName, _ref;
  _ref = bufferPath.split('/'), pumpName = _ref[0], bufferNames = 2 <= _ref.length ? __slice.call(_ref, 1) : [];
  bufferName = bufferNames.length ? bufferNames.join('/') : 'output';
  return this.pump(pumpName).buffer(bufferName);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Group.prototype.abort"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>abort ()](#apidoc.element.datapumps.Group.prototype.abort)
- description and source-code
```javascript
abort = function () {
  var name, pump;
  if (this._state !== Pump.STARTED) {
    throw new Error('Cannot .abort() a group that is not running');
  }
  return Promise.all((function() {
    var _ref, _results;
    _ref = this._pumps;
    _results = [];
    for (name in _ref) {
      pump = _ref[name];
      if (pump.isStarted()) {
        _results.push(pump.abort());
      }
    }
    return _results;
  }).call(this)).then((function(_this) {
    return function() {
      return _this._state = Group.ABORTED;
    };
  })(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Group.prototype.addInputPump"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>addInputPump (name, pump)](#apidoc.element.datapumps.Group.prototype.addInputPump)
- description and source-code
```javascript
addInputPump = function (name, pump) {
  var result;
  if (pump == null) {
    pump = null;
  }
  result = this.addPump(name, pump);
  this.inputPump(name);
  return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Group.prototype.addPump"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>addPump (name, pump)](#apidoc.element.datapumps.Group.prototype.addPump)
- description and source-code
```javascript
addPump = function (name, pump) {
  var pumpId;
  if (pump == null) {
    pump = null;
  }
  if (this._pumps[name] != null) {
    throw new Error('Pump already exists');
  }
  this._pumps[name] = pump != null ? pump : new Pump;
  pumpId = this._id != null ? "" + this._id + "/" + name : name;
  this._pumps[name].id(pumpId);
  this._pumps[name].errorBuffer(this._errorBuffer);
  return this._pumps[name];
}
```
- example usage
```shell
...
'''

## Pump group
You often need multiple pumps to complete an ETL task. Pump groups help starting multiple pump in
one step, and also enables handling the event when every pump ended:
'''js
sendMails = datapumps.group();
sendMails.addPump('tickets')
...;
sendMails.addPump('reminderMailer')
...;
sendMails
.start()
.whenFinished().then(function() {
  console.log('Tickets processed.');
...
```

#### <a name="apidoc.element.datapumps.Group.prototype.buffer"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>buffer (name)](#apidoc.element.datapumps.Group.prototype.buffer)
- description and source-code
```javascript
buffer = function (name) {
  var result, _ref;
  if (name == null) {
    name = 'output';
  }
  try {
    result = (_ref = this._exposedBuffers[name]) != null ? _ref : this._getBufferByPath(name);
  } catch (_error) {

  }
  if (!result) {
    throw new Error("No such buffer: " + name);
  }
  return result;
}
```
- example usage
```shell
...
'''js
datapumps = require('datapumps');
(pump = new datapumps.Pump())
  .from(<put a nodejs stream or datapumps buffer here>)
  .run()
'''

To access the output buffer, use the '.buffer()' method, which returns a Buffer instance:
'''js
buffer = pump.buffer('output');
buffer = pump.buffer(); // equivalent with previous as the default buffer
                        // of the pump is called 'output'
'''

Use the '.buffers()' method when you need to write data into multiple output buffers:
...
```

#### <a name="apidoc.element.datapumps.Group.prototype.constructor"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>constructor ()](#apidoc.element.datapumps.Group.prototype.constructor)
- description and source-code
```javascript
function Group() {
  Group.__super__.constructor.call(this);
  this._pumps = {};
  this._exposedBuffers = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Group.prototype.debugMode"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>debugMode (_debug)](#apidoc.element.datapumps.Group.prototype.debugMode)
- description and source-code
```javascript
debugMode = function (_debug) {
  this._debug = _debug;
  if (this._state !== Pump.STOPPED) {
    throw new Error('Cannot change debug mode after pump start');
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Group.prototype.expose"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>expose (exposedName, bufferPath)](#apidoc.element.datapumps.Group.prototype.expose)
- description and source-code
```javascript
expose = function (exposedName, bufferPath) {
  if (this._exposedBuffers[exposedName] != null) {
    throw new Error("Already exposed a buffer with name " + exposedName);
  }
  return this._exposedBuffers[exposedName] = this._getBufferByPath(bufferPath);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Group.prototype.from"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>from (buffer)](#apidoc.element.datapumps.Group.prototype.from)
- description and source-code
```javascript
from = function (buffer) {
  if (buffer == null) {
    buffer = null;
  }
  if (this._inputPump == null) {
    throw new Error('Input pump is not set, use .inputPump to set it');
  }
  this._inputPump.from(buffer);
  return this;
}
```
- example usage
```shell
...
MongodbMixin = datapumps.mixin.MongodbMixin,
ExcelWriterMixin = datapumps.mixin.ExcelWriterMixin,
pump = new Pump();

pump
.mixin(MongodbMixin('mongodb://localhost/marketing'))
.useCollection('Contact')
.from(pump.find({ country: "US" }))

.mixin(ExcelWriterMixin())
.createWorkbook('/tmp/ContactsInUs.xlsx')
.createWorksheet('Contacts')
.writeHeaders(['Name', 'Email'])

.process(function(contact) {
...
```

#### <a name="apidoc.element.datapumps.Group.prototype.id"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>id (id)](#apidoc.element.datapumps.Group.prototype.id)
- description and source-code
```javascript
id = function (id) {
  var name, pump, _ref;
  if (id == null) {
    id = null;
  }
  if (id === null) {
    return this._id;
  }
  this._id = id;
  _ref = this._pumps;
  for (name in _ref) {
    pump = _ref[name];
    pump.id("" + this._id + "/" + name);
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Group.prototype.inputPump"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>inputPump (pumpName)](#apidoc.element.datapumps.Group.prototype.inputPump)
- description and source-code
```javascript
inputPump = function (pumpName) {
  if (pumpName == null) {
    pumpName = null;
  }
  if (pumpName == null) {
    return this._inputPump;
  }
  this._inputPump = this.pump(pumpName);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Group.prototype.mixin"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>mixin (mixins)](#apidoc.element.datapumps.Group.prototype.mixin)
- description and source-code
```javascript
mixin = function (mixins) {
  if (this._inputPump == null) {
    throw new Error('Input pump is not set, use .inputPump to set it');
  }
  this._inputPump.mixin(mixins);
  return this;
}
```
- example usage
```shell
...
datapumps = require('datapumps'),
Pump = datapumps.Pump,
MongodbMixin = datapumps.mixin.MongodbMixin,
ExcelWriterMixin = datapumps.mixin.ExcelWriterMixin,
pump = new Pump();

pump
.mixin(MongodbMixin('mongodb://localhost/marketing'))
.useCollection('Contact')
.from(pump.find({ country: "US" }))

.mixin(ExcelWriterMixin())
.createWorkbook('/tmp/ContactsInUs.xlsx')
.createWorksheet('Contacts')
.writeHeaders(['Name', 'Email'])
...
```

#### <a name="apidoc.element.datapumps.Group.prototype.pause"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>pause ()](#apidoc.element.datapumps.Group.prototype.pause)
- description and source-code
```javascript
pause = function () {
  var name, pausePromises, pump, _ref;
  if (this._state === Group.PAUSED) {
    return;
  }
  if (this._state !== Group.STARTED) {
    throw new Error('Cannot .pause() a group that is not pumping');
  }
  pausePromises = [];
  _ref = this._pumps;
  for (name in _ref) {
    pump = _ref[name];
    if (pump.isStarted()) {
      pausePromises.push(pump.pause());
    }
  }
  return Promise.all(pausePromises).then((function(_this) {
    return function() {
      return _this._state = Group.PAUSED;
    };
  })(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Group.prototype.process"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>process ()](#apidoc.element.datapumps.Group.prototype.process)
- description and source-code
```javascript
process = function () {
  throw new Error('Cannot call .process() on a group: data in a group is transformed by its pumps.');
}
```
- example usage
```shell
...
.from(pump.find({ country: "US" }))

.mixin(ExcelWriterMixin())
.createWorkbook('/tmp/ContactsInUs.xlsx')
.createWorksheet('Contacts')
.writeHeaders(['Name', 'Email'])

.process(function(contact) {
  return pump.writeRow([ contact.name, contact.email ]);
})
.logErrorsToConsole()
.run()
  .then(function() {
    console.log("Done writing contacts to file");
  });
...
```

#### <a name="apidoc.element.datapumps.Group.prototype.pump"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>pump (name)](#apidoc.element.datapumps.Group.prototype.pump)
- description and source-code
```javascript
pump = function (name) {
  if (this._pumps[name] == null) {
    throw new Error("Pump " + name + " does not exist");
  }
  return this._pumps[name];
}
```
- example usage
```shell
...
etlProcess = datapumps.group()
etlProcess
  .addPump 'notifier', new Notifier
    .from <node stream or datapumps buffer>

etlProcess
  .addPump 'logger'
    .from etlProcess.pump('notifier').buffer()
    .process (data) ->
      console.log "Email sent to #{data.name} (#{data.email})"
'''
Please note that you cannot use '.process' method on a group.

## Error handling
Errors may occur while data is transfered between systems. Most of the time, you don't want to stop
...
```

#### <a name="apidoc.element.datapumps.Group.prototype.pumps"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>pumps ()](#apidoc.element.datapumps.Group.prototype.pumps)
- description and source-code
```javascript
pumps = function () {
  return this._pumps;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Group.prototype.resume"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>resume ()](#apidoc.element.datapumps.Group.prototype.resume)
- description and source-code
```javascript
resume = function () {
  var name, pump, _ref;
  if (this._state !== Group.PAUSED) {
    throw new Error('Cannot .resume() a group that is not paused');
  }
  this._state = Group.STARTED;
  _ref = this._pumps;
  for (name in _ref) {
    pump = _ref[name];
    pump.resume();
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Group.prototype.run"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>run ()](#apidoc.element.datapumps.Group.prototype.run)
- description and source-code
```javascript
run = function () {
  var result;
  (result = this.runPumps())["catch"](function(PumpingFailedError, e) {});
  return result;
}
```
- example usage
```shell
...
 .createWorksheet('Contacts')
 .writeHeaders(['Name', 'Email'])

 .process(function(contact) {
   return pump.writeRow([ contact.name, contact.email ]);
 })
 .logErrorsToConsole()
 .run()
   .then(function() {
     console.log("Done writing contacts to file");
   });
'''

Usage example with more details:
* First, we create a pump and setup reading from mongodb
...
```

#### <a name="apidoc.element.datapumps.Group.prototype.runPumps"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>runPumps (pumps)](#apidoc.element.datapumps.Group.prototype.runPumps)
- description and source-code
```javascript
runPumps = function (pumps) {
  var finishPromises, pumpName, _i, _len;
  if (pumps == null) {
    pumps = null;
  }
  if (pumps == null) {
    pumps = this._getAllStoppedPumps();
  }
  if (typeof pumps === 'string') {
    pumps = [pumps];
  }
  finishPromises = [];
  for (_i = 0, _len = pumps.length; _i < _len; _i++) {
    pumpName = pumps[_i];
    finishPromises.push(this.pump(pumpName).start().whenFinished());
  }
  return Promise.all(finishPromises);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Group.prototype.start"></a>[function <span class="apidocSignatureSpan">datapumps.Group.prototype.</span>start ()](#apidoc.element.datapumps.Group.prototype.start)
- description and source-code
```javascript
start = function () {
  var name, pump, _ref;
  if (this._state !== Group.STOPPED) {
    throw new Error('Group already started');
  }
  this._state = Group.STARTED;
  this._registerErrorBufferEvents();
  _ref = this._pumps;
  for (name in _ref) {
    pump = _ref[name];
    pump.errorBuffer(this._errorBuffer);
    pump.debugMode(this._debug);
  }
  this.run().then((function(_this) {
    return function() {
      return _this._endGroup();
    };
  })(this))["catch"](function(PumpingFailedError, e) {});
  return this;
}
```
- example usage
```shell
...
'''
The argument of '.process()' is a function that will be executed after the pump reads a data item.
The function is executed in the context of the pump object, i.e. 'this' refers to the pump itself. The
function should return a Promise that fulfills when the data is processed (i.e. written into a buffer
or stored elsewhere).

### Start and end of pumping
A pump is started by calling the '.start()' method. The 'end' event will be emitted when the
input stream or buffer ended and all output buffers became empty.
'''js
pump.on('end', function() {
  console.log('Pumped everything, and all my output buffers are empty. Bye.')
})
'''
...
```



# <a name="apidoc.module.datapumps.Pump"></a>[module datapumps.Pump](#apidoc.module.datapumps.Pump)

#### <a name="apidoc.element.datapumps.Pump.Pump"></a>[function <span class="apidocSignatureSpan">datapumps.</span>Pump ()](#apidoc.element.datapumps.Pump.Pump)
- description and source-code
```javascript
function Pump() {
  this._state = Pump.STOPPED;
  this._from = null;
  this._id = null;
  this._errorBuffer = new Buffer;
  this._debug = false;
  this.buffers({
    output: new Buffer
  });
}
```
- example usage
```shell
...
   The '.logErrorsToConsole()' will log any error to the console, surprisingly. The pump will start
   on calling '.run()'. It returns a [promise](https://promisesaplus.com/) that resolves when the pump finished.

## Pump
A pump reads data from its input buffer or stream and copies it to the output buffer by default:
'''js
datapumps = require('datapumps');
(pump = new datapumps.Pump())
  .from(<put a nodejs stream or datapumps buffer here>)
  .run()
'''

To access the output buffer, use the '.buffer()' method, which returns a Buffer instance:
'''js
buffer = pump.buffer('output');
...
```

#### <a name="apidoc.element.datapumps.Pump.EventEmitter"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.</span>EventEmitter ()](#apidoc.element.datapumps.Pump.EventEmitter)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.init"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.</span>init ()](#apidoc.element.datapumps.Pump.init)
- description and source-code
```javascript
init = function () {
  this.domain = null;
  if (EventEmitter.usingDomains) {
    // if there is an active domain, then attach to it.
    domain = domain || require('domain');
    if (domain.active && !(this instanceof domain.Domain)) {
      this.domain = domain.active;
    }
  }

  if (!this._events || this._events === Object.getPrototypeOf(this)._events) {
    this._events = new EventHandlers();
    this._eventsCount = 0;
  }

  this._maxListeners = this._maxListeners || undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.listenerCount"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.</span>listenerCount (emitter, type)](#apidoc.element.datapumps.Pump.listenerCount)
- description and source-code
```javascript
listenerCount = function (emitter, type) {
  if (typeof emitter.listenerCount === 'function') {
    return emitter.listenerCount(type);
  } else {
    return listenerCount.call(emitter, type);
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.datapumps.Pump.prototype"></a>[module datapumps.Pump.prototype](#apidoc.module.datapumps.Pump.prototype)

#### <a name="apidoc.element.datapumps.Pump.prototype._outputBufferEnded"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>_outputBufferEnded ()](#apidoc.element.datapumps.Pump.prototype._outputBufferEnded)
- description and source-code
```javascript
_outputBufferEnded = function () {
  var allEnded, buffer, name, _ref, _ref1;
  allEnded = true;
  _ref = this._buffers;
  for (name in _ref) {
    buffer = _ref[name];
    if (!buffer.isEnded()) {
      allEnded = false;
    }
  }
  if (!allEnded) {
    return;
  }
  this._state = Pump.ENDED;
  if (this._debug) {
    console.log("" + ((new Date()).toISOString()) + " [" + ((_ref1 = this._id) != null ? _ref1 : '(root)') + "] Pump ended");
  }
  return this.emit('end');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.prototype._process"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>_process (data)](#apidoc.element.datapumps.Pump.prototype._process)
- description and source-code
```javascript
_process = function (data) {
  return this.copy(data);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.prototype._pump"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>_pump ()](#apidoc.element.datapumps.Pump.prototype._pump)
- description and source-code
```javascript
_pump = function () {
  if (this._from.isEnded()) {
    return this.sealOutputBuffers();
  }
  if (this._state === Pump.PAUSED || this._state === Pump.ABORTED) {
    return;
  }
  return (this.currentRead = this._from.readAsync()).cancellable().then((function(_this) {
    return function(data) {
      var _ref;
      _this.currentRead = null;
      _this._processing = _this._process(data, _this);
      if (!(((_ref = _this._processing) != null ? _ref.then : void 0) instanceof Function)) {
        _this._processing = void 0;
        throw new Error(".process() did not return a Promise");
      }
      _this._processing = Promise.resolve(_this._processing);
      return _this._processing.cancellable();
    };
  })(this))["catch"](Promise.CancellationError, function() {})["catch"]((function(_this) {
    return function(err) {
      return _this.writeError(err);
    };
  })(this)).done((function(_this) {
    return function() {
      return _this._pump();
    };
  })(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.prototype._registerErrorBufferEvents"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>_registerErrorBufferEvents ()](#apidoc.element.datapumps.Pump.prototype._registerErrorBufferEvents)
- description and source-code
```javascript
_registerErrorBufferEvents = function () {
  return this._errorBuffer.on('full', (function(_this) {
    return function() {
      if (_this._state === Pump.STARTED) {
        return _this.abort().then(function() {
          return _this.emit('error');
        });
      }
    };
  })(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.prototype.abort"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>abort ()](#apidoc.element.datapumps.Pump.prototype.abort)
- description and source-code
```javascript
abort = function () {
  var _ref;
  if (this._state === Pump.ABORTED) {
    return;
  }
  if (this._state !== Pump.STARTED) {
    throw new Error('Cannot .abort() a pump that is not running');
  }
  this._state = Pump.ABORTED;
  if ((_ref = this._processing) != null ? _ref.isPending() : void 0) {
    return this._processing.cancel()["catch"](function(err) {});
  } else {
    return Promise.resolve();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.prototype.buffer"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>buffer (name, buffer)](#apidoc.element.datapumps.Pump.prototype.buffer)
- description and source-code
```javascript
buffer = function (name, buffer) {
  if (name == null) {
    name = 'output';
  }
  if (buffer == null) {
    buffer = null;
  }
  if (buffer === null) {
    if (!this._buffers[name]) {
      throw new Error("No such buffer: " + name);
    }
    return this._buffers[name];
  } else {
    if (this._state === Pump.STARTED) {
      throw new Error('Cannot change output buffers after pumping has been started');
    }
    if (!(buffer instanceof Buffer)) {
      throw new Error('buffer must be a datapumps.Buffer');
    }
    this._buffers[name] = buffer;
    return this;
  }
}
```
- example usage
```shell
...
'''js
datapumps = require('datapumps');
(pump = new datapumps.Pump())
  .from(<put a nodejs stream or datapumps buffer here>)
  .run()
'''

To access the output buffer, use the '.buffer()' method, which returns a Buffer instance:
'''js
buffer = pump.buffer('output');
buffer = pump.buffer(); // equivalent with previous as the default buffer
                        // of the pump is called 'output'
'''

Use the '.buffers()' method when you need to write data into multiple output buffers:
...
```

#### <a name="apidoc.element.datapumps.Pump.prototype.buffers"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>buffers (buffers)](#apidoc.element.datapumps.Pump.prototype.buffers)
- description and source-code
```javascript
buffers = function (buffers) {
  if (buffers == null) {
    buffers = null;
  }
  if (buffers === null) {
    return this._buffers;
  }
  if (this._state === Pump.STARTED) {
    throw new Error('Cannot change output buffers after pumping has been started');
  }
  this._buffers = buffers;
  return this;
}
```
- example usage
```shell
...
To access the output buffer, use the '.buffer()' method, which returns a Buffer instance:
'''js
buffer = pump.buffer('output');
buffer = pump.buffer(); // equivalent with previous as the default buffer
                      // of the pump is called 'output'
'''

Use the '.buffers()' method when you need to write data into multiple output buffers:
'''js
ticketsPump
.buffers({
  openTickets: ticketsPump.createBuffer(),
  closedTickets: ticketsPump.createBuffer(),
});
...
```

#### <a name="apidoc.element.datapumps.Pump.prototype.constructor"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>constructor ()](#apidoc.element.datapumps.Pump.prototype.constructor)
- description and source-code
```javascript
function Pump() {
  this._state = Pump.STOPPED;
  this._from = null;
  this._id = null;
  this._errorBuffer = new Buffer;
  this._debug = false;
  this.buffers({
    output: new Buffer
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.prototype.copy"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>copy (data, buffers)](#apidoc.element.datapumps.Pump.prototype.copy)
- description and source-code
```javascript
copy = function (data, buffers) {
  var buffer;
  if (buffers == null) {
    buffers = null;
  }
  if (buffers == null) {
    buffers = ['output'];
  }
  if (typeof buffers === 'string') {
    buffers = [buffers];
  }
  if (!Array.isArray(buffers)) {
    throw new Error('buffers must be an array of buffer names or a single buffers name');
  }
  if (buffers.length === 1) {
    return this.buffer(buffers[0]).writeAsync(data);
  } else {
    return Promise.all((function() {
      var _i, _len, _results;
      _results = [];
      for (_i = 0, _len = buffers.length; _i < _len; _i++) {
        buffer = buffers[_i];
        _results.push(this.buffer(buffer).writeAsync(data));
      }
      return _results;
    }).call(this));
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.prototype.createBuffer"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>createBuffer (options)](#apidoc.element.datapumps.Pump.prototype.createBuffer)
- description and source-code
```javascript
createBuffer = function (options) {
  if (options == null) {
    options = {};
  }
  return new Buffer(options);
}
```
- example usage
```shell
...
                      // of the pump is called 'output'
'''

Use the '.buffers()' method when you need to write data into multiple output buffers:
'''js
ticketsPump
.buffers({
  openTickets: ticketsPump.createBuffer(),
  closedTickets: ticketsPump.createBuffer(),
});

reminderMailer = new datapumps.Pump()
reminderMailer
.from(ticketPump.buffer('openTickets'))
...
...
```

#### <a name="apidoc.element.datapumps.Pump.prototype.debug"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>debug ()](#apidoc.element.datapumps.Pump.prototype.debug)
- description and source-code
```javascript
debug = function () {
  this.debugMode(true);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.prototype.debugMode"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>debugMode (_debug)](#apidoc.element.datapumps.Pump.prototype.debugMode)
- description and source-code
```javascript
debugMode = function (_debug) {
  this._debug = _debug;
  if (this._state !== Pump.STOPPED) {
    throw new Error('Cannot change debug mode after pump start');
  }
  if (this._debug) {
    this.mixin(BufferDebugMixin);
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.prototype.errorBuffer"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>errorBuffer (buffer)](#apidoc.element.datapumps.Pump.prototype.errorBuffer)
- description and source-code
```javascript
errorBuffer = function (buffer) {
  if (buffer == null) {
    buffer = null;
  }
  if (buffer === null) {
    return this._errorBuffer;
  }
  this._errorBuffer = buffer;
  return this;
}
```
- example usage
```shell
...
    console.log "Email sent to #{data.name} (#{data.email})"
'''
Please note that you cannot use '.process' method on a group.

## Error handling
Errors may occur while data is transfered between systems. Most of the time, you don't want to stop
on the first error but complete the transfer and re-run after fixing problems. Therefore
the pump group has an error buffer ('.errorBuffer()') which can hold ten error messages by default.
When the error buffer fills up, 'error' event is triggered and '.whenFinised()' promise is rejected:
'''js
group
.start()
.whenFinished()
  .then(function() {
    if (!group.errorBuffer().isEmpty()) {
...
```

#### <a name="apidoc.element.datapumps.Pump.prototype.from"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>from (buffer)](#apidoc.element.datapumps.Pump.prototype.from)
- description and source-code
```javascript
from = function (buffer) {
  if (buffer == null) {
    buffer = null;
  }
  if (buffer === null) {
    return this._from;
  }
  if (this._state === Pump.STARTED) {
    throw new Error('Cannot change source buffer after pumping has been started');
  }
  if (buffer instanceof Buffer) {
    this._from = buffer;
  } else if (buffer instanceof Pump) {
    this._from = buffer.buffer();
  } else if (buffer instanceof require('stream')) {
    this._from = new Buffer({
      size: 1000
    });
    buffer.on('data', (function(_this) {
      return function(data) {
        return _this._from.write(data);
      };
    })(this));
    buffer.on('end', (function(_this) {
      return function() {
        return _this._from.seal();
      };
    })(this));
    buffer.on('error', (function(_this) {
      return function(err) {
        return _this.writeError(err);
      };
    })(this));
    this._from.on('full', function() {
      return buffer.pause();
    });
    this._from.on('release', function() {
      return buffer.resume();
    });
  } else if (buffer instanceof Array) {
    this._from = new Buffer({
      content: buffer.slice(0),
      sealed: true
    });
  } else {
    throw new Error('Argument must be datapumps.Buffer or stream');
  }
  this._from.on('end', (function(_this) {
    return function() {
      return _this.sourceEnded();
    };
  })(this));
  return this;
}
```
- example usage
```shell
...
MongodbMixin = datapumps.mixin.MongodbMixin,
ExcelWriterMixin = datapumps.mixin.ExcelWriterMixin,
pump = new Pump();

pump
.mixin(MongodbMixin('mongodb://localhost/marketing'))
.useCollection('Contact')
.from(pump.find({ country: "US" }))

.mixin(ExcelWriterMixin())
.createWorkbook('/tmp/ContactsInUs.xlsx')
.createWorksheet('Contacts')
.writeHeaders(['Name', 'Email'])

.process(function(contact) {
...
```

#### <a name="apidoc.element.datapumps.Pump.prototype.id"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>id (id)](#apidoc.element.datapumps.Pump.prototype.id)
- description and source-code
```javascript
id = function (id) {
  if (id == null) {
    id = null;
  }
  if (id === null) {
    return this._id;
  }
  this._id = id;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.prototype.isEnded"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>isEnded ()](#apidoc.element.datapumps.Pump.prototype.isEnded)
- description and source-code
```javascript
isEnded = function () {
  return this._state === Pump.ENDED;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.prototype.isPaused"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>isPaused ()](#apidoc.element.datapumps.Pump.prototype.isPaused)
- description and source-code
```javascript
isPaused = function () {
  return this._state === Pump.PAUSED;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.prototype.isStarted"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>isStarted ()](#apidoc.element.datapumps.Pump.prototype.isStarted)
- description and source-code
```javascript
isStarted = function () {
  return this._state === Pump.STARTED;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.prototype.isStopped"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>isStopped ()](#apidoc.element.datapumps.Pump.prototype.isStopped)
- description and source-code
```javascript
isStopped = function () {
  return this._state === Pump.STOPPED;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.prototype.logErrorsToConsole"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>logErrorsToConsole ()](#apidoc.element.datapumps.Pump.prototype.logErrorsToConsole)
- description and source-code
```javascript
logErrorsToConsole = function () {
  this.errorBuffer().on('write', (function(_this) {
    return function(errorRecord) {
      var name, _ref, _ref1;
      name = (_ref = errorRecord.pump) != null ? _ref : '(root)';
      if (_this._debug) {
        console.log("Error in pump " + name + ":");
        return console.log((_ref1 = errorRecord.error.stack) != null ? _ref1 : errorRecord.error);
      } else {
        return console.log("Error in pump " + name + ": " + errorRecord.error);
      }
    };
  })(this));
  return this;
}
```
- example usage
```shell
...
  .createWorkbook('/tmp/ContactsInUs.xlsx')
  .createWorksheet('Contacts')
  .writeHeaders(['Name', 'Email'])

  .process(function(contact) {
    return pump.writeRow([ contact.name, contact.email ]);
  })
  .logErrorsToConsole()
  .run()
    .then(function() {
      console.log("Done writing contacts to file");
    });
'''

Usage example with more details:
...
```

#### <a name="apidoc.element.datapumps.Pump.prototype.mixin"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>mixin (mixins)](#apidoc.element.datapumps.Pump.prototype.mixin)
- description and source-code
```javascript
mixin = function (mixins) {
  var mixin, _i, _len;
  mixins = Array.isArray(mixins) ? mixins : [mixins];
  for (_i = 0, _len = mixins.length; _i < _len; _i++) {
    mixin = mixins[_i];
    mixin(this);
  }
  return this;
}
```
- example usage
```shell
...
datapumps = require('datapumps'),
Pump = datapumps.Pump,
MongodbMixin = datapumps.mixin.MongodbMixin,
ExcelWriterMixin = datapumps.mixin.ExcelWriterMixin,
pump = new Pump();

pump
.mixin(MongodbMixin('mongodb://localhost/marketing'))
.useCollection('Contact')
.from(pump.find({ country: "US" }))

.mixin(ExcelWriterMixin())
.createWorkbook('/tmp/ContactsInUs.xlsx')
.createWorksheet('Contacts')
.writeHeaders(['Name', 'Email'])
...
```

#### <a name="apidoc.element.datapumps.Pump.prototype.pause"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>pause ()](#apidoc.element.datapumps.Pump.prototype.pause)
- description and source-code
```javascript
pause = function () {
  var _ref;
  if (this._state === Pump.PAUSED) {
    return;
  }
  if (this._state !== Pump.STARTED) {
    throw new Error('Cannot .pause() a pump that is not running');
  }
  if ((_ref = this._processing) != null ? _ref.isPending() : void 0) {
    return this._processing.then((function(_this) {
      return function() {
        return _this._state = Pump.PAUSED;
      };
    })(this));
  } else {
    this._state = Pump.PAUSED;
    return Promise.resolve();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.prototype.process"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>process (fn)](#apidoc.element.datapumps.Pump.prototype.process)
- description and source-code
```javascript
process = function (fn) {
  if (typeof fn !== 'function') {
    throw new Error('.process() argument must be a Promise returning function ');
  }
  this._process = fn;
  return this;
}
```
- example usage
```shell
...
.from(pump.find({ country: "US" }))

.mixin(ExcelWriterMixin())
.createWorkbook('/tmp/ContactsInUs.xlsx')
.createWorksheet('Contacts')
.writeHeaders(['Name', 'Email'])

.process(function(contact) {
  return pump.writeRow([ contact.name, contact.email ]);
})
.logErrorsToConsole()
.run()
  .then(function() {
    console.log("Done writing contacts to file");
  });
...
```

#### <a name="apidoc.element.datapumps.Pump.prototype.resume"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>resume ()](#apidoc.element.datapumps.Pump.prototype.resume)
- description and source-code
```javascript
resume = function () {
  if (this._state !== Pump.PAUSED) {
    throw new Error('Cannot .resume() a pump that is not paused');
  }
  this._state = Pump.STARTED;
  this._pump();
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.prototype.run"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>run ()](#apidoc.element.datapumps.Pump.prototype.run)
- description and source-code
```javascript
run = function () {
  return this.start().whenFinished();
}
```
- example usage
```shell
...
 .createWorksheet('Contacts')
 .writeHeaders(['Name', 'Email'])

 .process(function(contact) {
   return pump.writeRow([ contact.name, contact.email ]);
 })
 .logErrorsToConsole()
 .run()
   .then(function() {
     console.log("Done writing contacts to file");
   });
'''

Usage example with more details:
* First, we create a pump and setup reading from mongodb
...
```

#### <a name="apidoc.element.datapumps.Pump.prototype.sealOutputBuffers"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>sealOutputBuffers ()](#apidoc.element.datapumps.Pump.prototype.sealOutputBuffers)
- description and source-code
```javascript
sealOutputBuffers = function () {
  var buffer, name, _ref, _results;
  _ref = this._buffers;
  _results = [];
  for (name in _ref) {
    buffer = _ref[name];
    if (!buffer.isSealed()) {
      _results.push(buffer.seal());
    } else {
      _results.push(void 0);
    }
  }
  return _results;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.prototype.sourceEnded"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>sourceEnded ()](#apidoc.element.datapumps.Pump.prototype.sourceEnded)
- description and source-code
```javascript
sourceEnded = function () {
  if (this.currentRead) {
    return this.currentRead.cancel();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.prototype.start"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>start ()](#apidoc.element.datapumps.Pump.prototype.start)
- description and source-code
```javascript
start = function () {
  var buffer, name, _ref, _ref1;
  if (!this._from) {
    throw new Error('Source is not configured');
  }
  if (this._state !== Pump.STOPPED) {
    throw new Error('Pump is already started');
  }
  if (this._debug) {
    console.log("" + ((new Date()).toISOString()) + " [" + ((_ref = this._id) != null ? _ref : '(root)') + "] Pump started");
  }
  this._state = Pump.STARTED;
  this._registerErrorBufferEvents();
  _ref1 = this._buffers;
  for (name in _ref1) {
    buffer = _ref1[name];
    buffer.on('end', this._outputBufferEnded.bind(this));
  }
  this._pump();
  return this;
}
```
- example usage
```shell
...
'''
The argument of '.process()' is a function that will be executed after the pump reads a data item.
The function is executed in the context of the pump object, i.e. 'this' refers to the pump itself. The
function should return a Promise that fulfills when the data is processed (i.e. written into a buffer
or stored elsewhere).

### Start and end of pumping
A pump is started by calling the '.start()' method. The 'end' event will be emitted when the
input stream or buffer ended and all output buffers became empty.
'''js
pump.on('end', function() {
  console.log('Pumped everything, and all my output buffers are empty. Bye.')
})
'''
...
```

#### <a name="apidoc.element.datapumps.Pump.prototype.to"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>to (pump, bufferName)](#apidoc.element.datapumps.Pump.prototype.to)
- description and source-code
```javascript
to = function (pump, bufferName) {
  pump.from(this.buffer(bufferName));
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.Pump.prototype.whenFinished"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>whenFinished ()](#apidoc.element.datapumps.Pump.prototype.whenFinished)
- description and source-code
```javascript
whenFinished = function () {
  if (this.isEnded()) {
    return Promise.resolve();
  }
  return new Promise((function(_this) {
    return function(resolve, reject) {
      _this.on('end', function() {
        return resolve();
      });
      return _this.on('error', function() {
        return reject(new PumpingFailedError());
      });
    };
  })(this));
}
```
- example usage
```shell
...
sendMails = datapumps.group();
sendMails.addPump('tickets')
  ...;
sendMails.addPump('reminderMailer')
  ...;
sendMails
  .start()
  .whenFinished().then(function() {
    console.log('Tickets processed.');
  });
'''
The '.addPump()' method creates a new pump with given name and returns it for configuration.
'.start()' will start all pumps in the group, while '.whenFinished()' returns a Promise the fulfills
when every pump ended (Note: 'end' event is also emitted).
...
```

#### <a name="apidoc.element.datapumps.Pump.prototype.writeError"></a>[function <span class="apidocSignatureSpan">datapumps.Pump.prototype.</span>writeError (err)](#apidoc.element.datapumps.Pump.prototype.writeError)
- description and source-code
```javascript
writeError = function (err) {
  if (this._errorBuffer.isFull()) {
    return;
  }
  this._errorBuffer.write({
    error: err,
    pump: this._id
  });
  return this;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.datapumps.PumpingFailedError"></a>[module datapumps.PumpingFailedError](#apidoc.module.datapumps.PumpingFailedError)

#### <a name="apidoc.element.datapumps.PumpingFailedError.PumpingFailedError"></a>[function <span class="apidocSignatureSpan">datapumps.</span>PumpingFailedError (message)](#apidoc.element.datapumps.PumpingFailedError.PumpingFailedError)
- description and source-code
```javascript
function PumpingFailedError(message) {
  this.message = message != null ? message : 'Pumping failed. See .errorBuffer() contents for error messages';
  PumpingFailedError.__super__.constructor.call(this, this.message);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.PumpingFailedError.captureStackTrace"></a>[function <span class="apidocSignatureSpan">datapumps.PumpingFailedError.</span>captureStackTrace ()](#apidoc.element.datapumps.PumpingFailedError.captureStackTrace)
- description and source-code
```javascript
function captureStackTrace() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.datapumps.PumpingFailedError.prototype"></a>[module datapumps.PumpingFailedError.prototype](#apidoc.module.datapumps.PumpingFailedError.prototype)

#### <a name="apidoc.element.datapumps.PumpingFailedError.prototype.constructor"></a>[function <span class="apidocSignatureSpan">datapumps.PumpingFailedError.prototype.</span>constructor (message)](#apidoc.element.datapumps.PumpingFailedError.prototype.constructor)
- description and source-code
```javascript
function PumpingFailedError(message) {
  this.message = message != null ? message : 'Pumping failed. See .errorBuffer() contents for error messages';
  PumpingFailedError.__super__.constructor.call(this, this.message);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.datapumps.mixin"></a>[module datapumps.mixin](#apidoc.module.datapumps.mixin)

#### <a name="apidoc.element.datapumps.mixin.BatchMixin"></a>[function <span class="apidocSignatureSpan">datapumps.mixin.</span>BatchMixin (target)](#apidoc.element.datapumps.mixin.BatchMixin)
- description and source-code
```javascript
BatchMixin = function (target) {
  var pumpMethod;
  target._batchSize = 100;
  target._batch = [];
  target.batchSize = function(size) {
    if (size == null) {
      return this._batchSize;
    }
    if (size <= 1) {
      throw new Error("Invalid batch size: " + size);
    }
    this._batchSize = size;
    return this;
  };
  target.processBatch = function(fn) {
    if (typeof fn !== 'function') {
      throw new Error('processBatch argument must be a function');
    }
    this._processBatch = fn;
    return this;
  };
  target._process = function(data) {
    var result;
    this._batch.push(data);
    if (this._batch.length >= this._batchSize) {
      result = this._processBatch(this._batch);
      this._batch = [];
      return result;
    } else {
      return Promise.resolve();
    }
  };
  pumpMethod = target._pump;
  return target._pump = function() {
    if (this._from.isEnded()) {
      if (this._batch.length > 0) {
        Promise.resolve(this._processBatch(this._batch))["catch"]((function(_this) {
          return function(err) {
            return _this.writeError(err);
          };
        })(this)).then((function(_this) {
          return function() {
            return _this.sealOutputBuffers();
          };
        })(this));
      } else {
        this.sealOutputBuffers();
      }
      this._batch = [];
      return;
    }
    return pumpMethod.apply(target, []);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.mixin.BufferDebugMixin"></a>[function <span class="apidocSignatureSpan">datapumps.mixin.</span>BufferDebugMixin (pump)](#apidoc.element.datapumps.mixin.BufferDebugMixin)
- description and source-code
```javascript
BufferDebugMixin = function (pump) {
  var clearBufferStats, collectBuffers, delay, dumpStats, dumpStatsIfNotEnded, hadTraffic, listenToBuffersEvents, monitorBuffers
, _bufferStats, _start;
  if ('_bufferDebugMixin' in pump) {
    return;
  }
  _start = pump.start;
  _bufferStats = {};
  pump._bufferDebugMixin = {
    version: 1
  };
  pump.start = function() {
    _start.call(pump);
    if (this._debug !== true) {
      return this;
    }
    collectBuffers();
    listenToBuffersEvents();
    monitorBuffers();
    pump.whenFinished().then(function() {
      return dumpStats();
    });
    return this;
  };
  collectBuffers = function() {
    var buffer, name, _ref;
    _bufferStats = {
      input: {
        buffer: pump.from()
      }
    };
    _ref = pump.buffers();
    for (name in _ref) {
      buffer = _ref[name];
      _bufferStats[name] = {
        buffer: buffer
      };
    }
    return clearBufferStats();
  };
  clearBufferStats = function() {
    var buffer, name, _results;
    _results = [];
    for (name in _bufferStats) {
      buffer = _bufferStats[name];
      buffer.releases = 0;
      _results.push(buffer.writes = 0);
    }
    return _results;
  };
  listenToBuffersEvents = function() {
    var buffer, name, _results;
    _results = [];
    for (name in _bufferStats) {
      buffer = _bufferStats[name];
      _results.push((function(buffer) {
        if (!buffer.buffer) {
          return;
        }
        buffer.buffer.on('write', function() {
          return buffer.writes++;
        });
        return buffer.buffer.on('release', function() {
          return buffer.releases++;
        });
      })(buffer));
    }
    return _results;
  };
  monitorBuffers = function() {
    return delay(1000, function() {
      dumpStatsIfNotEnded();
      clearBufferStats();
      if (!pump.isEnded()) {
        return monitorBuffers();
      }
    });
  };
  delay = function(ms, func) {
    return setTimeout(func, ms);
  };
  dumpStatsIfNotEnded = function() {
    if (pump.isEnded()) {
      return;
    }
    return dumpStats();
  };
  dumpStats = function() {
    var buffer, name, _ref;
    if (!hadTraffic()) {
      return;
    }
    process.stdout.write("" + ((new Date()).toISOString()) + " [" + ((_ref = pump.id()) != null ? _ref : '(root)') + "] ");
    for (name in _bufferStats) {
      buffer = _bufferStats[name];
      process.stdout.write("" + name + ": " + (buffer.buffer.getContent().length) + " items, " + buffer.writes + " in, " + buffer
.releases + " out | ");
    }
    return process.stdout.write("\n");
  };
  return hadTraffic = function() {
    var buffer, name;
    for (name in _bufferStats) {
      buffer = _bufferStats[name];
      if (buffer.releases > 0 || buffer.writes > 0) {
        return true;
      }
    }
    return false;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.mixin.CsvWriterMixin"></a>[function <span class="apidocSignatureSpan">datapumps.mixin.</span>CsvWriterMixin (options)](#apidoc.element.datapumps.mixin.CsvWriterMixin)
- description and source-code
```javascript
CsvWriterMixin = function (options) {
  if (!(options != null ? options.path : void 0)) {
    throw new Error('path option is required.');
  }
  return function(target) {
    target.writeRow = function(row) {
      return target._csv.writer.writeAsync(row);
    };
    target._csv = options;
    target._csv.writer = Promise.promisifyAll(csv.createWriteStream());
    target._csv.writer.pipe(fs.createWriteStream(target._csv.path, {
      encoding: 'utf8'
    }));
    if (target._csv.headers != null) {
      target.writeRow(target._csv.headers);
    }
    return target.on('end', function() {
      return target._csv.writer.write(null);
    });
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.mixin.ExcelReaderMixin"></a>[function <span class="apidocSignatureSpan">datapumps.mixin.</span>ExcelReaderMixin (_arg)](#apidoc.element.datapumps.mixin.ExcelReaderMixin)
- description and source-code
```javascript
ExcelReaderMixin = function (_arg) {
  var columnMapping, path, worksheet;
  worksheet = _arg.worksheet, columnMapping = _arg.columnMapping, path = _arg.path;
  return function(target) {
    var buffer, content, data, mapColumnNames, workbook, _i, _len, _ref2;
    if (path != null) {
      workbook = readFile(path);
      worksheet = workbook.Sheets[worksheet];
    }
    if (worksheet == null) {
      throw new Error('worksheet property is required for ExcelReaderMixin');
    }
    target._excel = {
      worksheet: worksheet,
      columnMapping: columnMapping
    };
    mapColumnNames = function(data) {
      var from, result, to;
      result = {};
      for (from in columnMapping) {
        to = columnMapping[from];
        result[to] = data[from];
      }
      return result;
    };
    content = [];
    if (columnMapping) {
      _ref2 = convertSheetToJson(worksheet);
      for (_i = 0, _len = _ref2.length; _i < _len; _i++) {
        data = _ref2[_i];
        content.push(mapColumnNames(data));
      }
    } else {
      content = convertSheetToJson(worksheet);
    }
    buffer = new Buffer({
      content: content
    });
    target.from(buffer);
    return buffer.seal();
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.mixin.ExcelWriterMixin"></a>[function <span class="apidocSignatureSpan">datapumps.mixin.</span>ExcelWriterMixin (onMixin)](#apidoc.element.datapumps.mixin.ExcelWriterMixin)
- description and source-code
```javascript
ExcelWriterMixin = function (onMixin) {
  return function(target) {
    target._excel = {
      columnTypes: [],
      path: null
    };
    target.createWorkbook = function(path) {
      if (this._excel.workbook != null) {
        throw new Error('Workbook already created');
      }
      this.workbook(new excel4node.WorkBook());
      this._excel.path = path;
      this.on('end', (function(_this) {
        return function() {
          return _this._excel.workbook.write(_this._excel.path);
        };
      })(this));
      this._excel.workbook;
      return this;
    };
    target.workbook = function(workbook) {
      if (workbook == null) {
        workbook = null;
      }
      if (workbook === null) {
        return this._excel.workbook;
      }
      this._excel.workbook = workbook;
      this._excel.boldStyle = this._excel.workbook.Style();
      this._excel.boldStyle.Font.Bold();
      return this;
    };
    target.createWorksheet = function(name) {
      if (this._excel.workbook == null) {
        throw new Error('Use createWorkbook before creating worksheet');
      }
      this._excel.worksheet = this._excel.workbook.WorkSheet(name);
      this._excel.currentRow = 1;
      return this;
    };
    target.currentWorksheet = function() {
      return this._excel.worksheet;
    };
    target.writeHeaders = function(headers, types) {
      var header, index, _i, _len, _ref;
      if (types == null) {
        types = [];
      }
      if (this._excel.worksheet == null) {
        throw new Error('Use createWorksheet before writing headers');
      }
      if (this._excel.currentRow !== 1) {
        throw new Error('Use writeHeaders before writing any rows to the worksheet');
      }
      for (index = _i = 0, _len = headers.length; _i < _len; index = ++_i) {
        header = headers[index];
        this._writeHeader(index, header);
        this.columnType(index, (_ref = types[index]) != null ? _ref : 'String');
      }
      this._excel.currentRow = 2;
      return this;
    };
    target._writeHeader = function(index, header) {
      this._excel.worksheet.Cell(1, index + 1).String(header).Style(this._excel.boldStyle);
      return this;
    };
    target.columnType = function(index, type) {
      if (type == null) {
        type = null;
      }
      if (type === null) {
        return this._excel.columnTypes[index];
      }
      if (['String', 'Number', 'Formula'].indexOf(type) === -1) {
        throw new Error("Invalid column type '" + type + "'. Only String, Number or Formula is allowed");
      }
      this._excel.columnTypes[index] = type;
      return this;
    };
    target.writeRow = function(columns) {
      var cell, index, value, _i, _len, _ref;
      if (this._excel.worksheet == null) {
        throw new Error('Use createWorksheet before writing rows');
      }
      for (index = _i = 0, _len = columns.length; _i < _len; index = ++_i) {
        value = columns[index];
        if (value === null || value === void 0) {
          continue;
        }
        cell = this._excel.worksheet.Cell(this._excel.currentRow, index + 1);
        cell[(_ref = this._excel.columnTypes[index]) != null ? _ref : 'String'](value);
      }
      this._excel.currentRow++;
      return Promise.resolve();
    };
    if (onMixin) {
      return onMixin.apply(target, [target]);
    }
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.mixin.MergeMixin"></a>[function <span class="apidocSignatureSpan">datapumps.mixin.</span>MergeMixin (pump)](#apidoc.element.datapumps.mixin.MergeMixin)
- description and source-code
```javascript
MergeMixin = function (pump) {
  pump.from(new Buffer());
  pump._fromBuffers = [];
  return pump.from = function(buffer) {
    var helperPump, sourceBuffer;
    if (buffer == null) {
      buffer = null;
    }
    if (buffer === null) {
      return this._from;
    }
    if (this._state === Pump.STARTED) {
      throw new Error('Cannot change source buffer after pumping has been started');
    }
    if (buffer instanceof Buffer) {
      sourceBuffer = buffer;
    } else if (buffer instanceof Pump) {
      sourceBuffer = buffer.buffer();
    } else if (buffer instanceof require('stream')) {
      sourceBuffer = new Buffer({
        size: 1000
      });
      buffer.on('data', (function(_this) {
        return function(data) {
          return sourceBuffer.write(data);
        };
      })(this));
      buffer.on('end', (function(_this) {
        return function() {
          return sourceBuffer.seal();
        };
      })(this));
      buffer.on('error', (function(_this) {
        return function(err) {
          return _this.writeError(err);
        };
      })(this));
      sourceBuffer.on('full', function() {
        return buffer.pause();
      });
      sourceBuffer.on('release', function() {
        return buffer.resume();
      });
    } else {
      throw new Error('Argument must be datapumps.Buffer or stream');
    }
    this._fromBuffers.push(sourceBuffer);
    (helperPump = new MergeHelperPump()).from(sourceBuffer).buffer('output', this._from).process(function(data) {
      return this.copy(data);
    });
    helperPump.on('sealOutput', function() {
      var allEnded, _i, _len, _ref;
      allEnded = true;
      _ref = pump._fromBuffers;
      for (_i = 0, _len = _ref.length; _i < _len; _i++) {
        buffer = _ref[_i];
        if (!buffer.isEnded()) {
          allEnded = false;
        }
      }
      if (!allEnded) {
        return;
      }
      if (!pump._from.isSealed()) {
        return pump._from.seal();
      }
    }).start();
    return this;
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.mixin.MongodbMixin"></a>[function <span class="apidocSignatureSpan">datapumps.mixin.</span>MongodbMixin (db)](#apidoc.element.datapumps.mixin.MongodbMixin)
- description and source-code
```javascript
MongodbMixin = function (db) {
  return function(target) {
    var name, _i, _len;
    target._mongo = {
      db: db
    };
    if (typeof db === 'string') {
      (target._mongo.whenConnected = mongo.MongoClient.connectAsync(db)).then(function(db) {
        var _ref, _ref1;
        target._mongo.db = db;
        target.whenFinished().then(function() {
          return target._mongo.db.close();
        });
        if (((_ref = target._mongo) != null ? (_ref1 = _ref.collection) != null ? _ref1._datapumpsMixinName : void 0 : void 0) !=
null) {
          return target._mongo.collection = db.collection(target._mongo.collection._datapumpsMixinName);
        }
      });
    }
    for (_i = 0, _len = _wrappedMethods.length; _i < _len; _i++) {
      name = _wrappedMethods[_i];
      _wrapMethod(target, name);
    }
    _wrapFind(target);
    target.setGlobalDefaultMaxBsonSize = function(size) {
      require('mongodb').Connection.DEFAULT_MAX_BSON_SIZE = size;
      require('mongodb').Connection.DEFAULT_MAX_MESSAGE_SIZE = size;
      return this;
    };
    target.db = function() {
      return this._mongo.db;
    };
    target.useCollection = function(name) {
      var _j, _len1, _ref;
      if ((target._mongo.whenConnected != null) && ((_ref = target._mongo) != null ? _ref.whenConnected.isPending() : void 0)) {
        this._mongo.collection = {
          _datapumpsMixinName: name
        };
        for (_j = 0, _len1 = _wrappedMethods.length; _j < _len1; _j++) {
          name = _wrappedMethods[_j];
          _deferCollectionMethod(this._mongo.collection, name + 'Async', this);
        }
        _deferFind(this._mongo.collection, this);
      } else {
        this._mongo.collection = this._mongo.db.collection(name);
      }
      return this;
    };
    return target.collection = function(name) {
      var _ref;
      if ((_ref = target._mongo) != null ? _ref.whenConnected.isPending() : void 0) {
        throw new Error('Not yet connected to mongo');
      }
      return this._mongo.db.collection(name);
    };
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.mixin.MysqlMixin"></a>[function <span class="apidocSignatureSpan">datapumps.mixin.</span>MysqlMixin (connection)](#apidoc.element.datapumps.mixin.MysqlMixin)
- description and source-code
```javascript
MysqlMixin = function (connection) {
  if ((connection == null) || typeof (connection != null ? connection.query : void 0) !== 'function') {
    throw new Error('Mysql mixin requires connection to be given');
  }
  return function(target) {
    target._mysql = {
      connection: connection,
      query: Promise.promisify(connection.query, connection)
    };
    target.query = function() {
      var args, query;
      query = arguments[0], args = 2 <= arguments.length ? __slice.call(arguments, 1) : [];
      if (args != null) {
        return this._mysql.query(query, args);
      } else {
        return this._mysql.query(query);
      }
    };
    target.selectOne = function() {
      var args, query;
      query = arguments[0], args = 2 <= arguments.length ? __slice.call(arguments, 1) : [];
      return target.query(query, args).then(function(_arg) {
        var fields, results;
        results = _arg[0], fields = _arg[1];
        if (results.length === 1) {
          return results[0];
        } else if (results.length === 0) {
          throw new Error('Query returned no result');
        } else {
          throw new Error('Query returned more than one result');
        }
      });
    };
    return target.escape = function(value) {
      return this._mysql.connection.escape(value);
    };
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.mixin.ObjectTransformMixin"></a>[function <span class="apidocSignatureSpan">datapumps.mixin.</span>ObjectTransformMixin ()](#apidoc.element.datapumps.mixin.ObjectTransformMixin)
- description and source-code
```javascript
ObjectTransformMixin = function () {
  return function(target) {
    target.propertiesToLowerCase = function(data) {
      var prop, result, value;
      result = {};
      for (prop in data) {
        value = data[prop];
        result[prop.toLowerCase()] = value;
      }
      return result;
    };
    target.requireProperty = function(obj, properties) {
      var property, result, _i, _j, _len, _len1;
      properties = Array.isArray(properties) ? properties : [properties];
      for (_i = 0, _len = properties.length; _i < _len; _i++) {
        property = properties[_i];
        if (obj[property] == null) {
          throw new Error('Missing property: ' + property);
        }
      }
      if (properties.length === 1) {
        return obj[properties[0]];
      } else {
        result = {};
        for (_j = 0, _len1 = properties.length; _j < _len1; _j++) {
          property = properties[_j];
          result[property] = obj[property];
        }
        return result;
      }
    };
    return target.boolValueOf = function(obj) {
      return !(obj === null || obj === void 0 || obj === false || obj === 'off' || obj === 'false' || obj === 0 || obj === 'no');
    };
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.datapumps.mixin.RestMixin"></a>[function <span class="apidocSignatureSpan">datapumps.mixin.</span>RestMixin (target)](#apidoc.element.datapumps.mixin.RestMixin)
- description and source-code
```javascript
RestMixin = function (target) {
  _wrapMethod(target, 'get');
  _wrapMethod(target, 'post');
  _wrapMethod(target, 'put');
  _wrapMethod(target, 'del');
  _wrapMethod(target, 'head');
  _wrapMethod(target, 'patch');
  _wrapMethod(target, 'json');
  _wrapMethod(target, 'postJson');
  _wrapMethod(target, 'putJson');
  target.file = function() {
    return restler.file.apply(restler, arguments);
  };
  return target.fromRest = function(config) {
    var queryAndWriteInputBuffer;
    if (!(config != null ? config.query : void 0)) {
      throw new Error('query key is required');
    }
    if (config.resultMapping == null) {
      config.resultMapping = function(result) {
        return result;
      };
    }
    if (config.nextPage == null) {
      config.nextPage = function() {
        return void 0;
      };
    }
    this.from(this.createBuffer());
    queryAndWriteInputBuffer = (function(_this) {
      return function(nextPage) {
        return config.query.apply(_this, [nextPage]).then(function(response) {
          return _this.from().writeArrayAsync(config.resultMapping(response)).done(function() {
            nextPage = config.nextPage(response);
            if ((nextPage === void 0) || (nextPage === null)) {
              return _this.from().seal();
            } else {
              return queryAndWriteInputBuffer(nextPage);
            }
          });
        });
      };
    })(this);
    queryAndWriteInputBuffer(void 0);
    return this;
  };
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
