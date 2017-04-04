# api documentation for  [google-closure-compiler (v20170218.0.0)](https://developers.google.com/closure/compiler/)  [![npm package](https://img.shields.io/npm/v/npmdoc-google-closure-compiler.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-google-closure-compiler) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-google-closure-compiler.svg)](https://travis-ci.org/npmdoc/node-npmdoc-google-closure-compiler)
#### Check, compile, optimize and compress Javascript with Closure-Compiler

[![NPM](https://nodei.co/npm/google-closure-compiler.png?downloads=true)](https://www.npmjs.com/package/google-closure-compiler)

[![apidoc](https://npmdoc.github.io/node-npmdoc-google-closure-compiler/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-google-closure-compiler_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-google-closure-compiler/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-google-closure-compiler/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-google-closure-compiler/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/google/closure-compiler/issues"
    },
    "contributors": [
        {
            "name": "Chad Killingsworth",
            "email": "chadkillingsworth@gmail.com"
        }
    ],
    "dependencies": {
        "chalk": "^1.0.0",
        "vinyl": "^1.2.0",
        "vinyl-sourcemaps-apply": "^0.2.0"
    },
    "description": "Check, compile, optimize and compress Javascript with Closure-Compiler",
    "devDependencies": {
        "gulp": "^3.9.0",
        "gulp-mocha": "^2.2.0",
        "gulp-sourcemaps": "^1.6.0",
        "lodash": "^4.6.1",
        "mocha": "^2.3.4",
        "ncp": "^2.0.0",
        "semver": "^5.1.0",
        "should": "^8.2.2",
        "stream-assert": "^2.0.3",
        "vinyl": "^1.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "059c7f91cf1cb2c1a66b4c95f745f5efd0fb4ba4",
        "tarball": "https://registry.npmjs.org/google-closure-compiler/-/google-closure-compiler-20170218.0.0.tgz"
    },
    "engines": {
        "node": ">=0.12.0"
    },
    "files": [
        "lib/",
        "compiler.jar",
        "index.js",
        "package.json",
        "contrib/",
        "README.md"
    ],
    "gitHead": "04be31afc7f1f118cfc4dd701079019ee3b2ac8e",
    "homepage": "https://developers.google.com/closure/compiler/",
    "keywords": [
        "javascript",
        "compiler",
        "optimizer",
        "minifier",
        "closure",
        "gulpplugin",
        "gruntplugin"
    ],
    "license": "Apache-2.0",
    "main": "index.js",
    "maintainers": [
        {
            "name": "blickly",
            "email": "blickly+npm@google.com"
        },
        {
            "name": "brad4d",
            "email": "bradfordcsmith@google.com"
        },
        {
            "name": "chadhikes",
            "email": "chadkillingsworth@gmail.com"
        },
        {
            "name": "dominator008",
            "email": "zhoumotongxue008@gmail.com"
        },
        {
            "name": "joeltine",
            "email": "jmarti221@gmail.com"
        }
    ],
    "name": "google-closure-compiler",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/google/closure-compiler-npm.git"
    },
    "scripts": {
        "pretest": "./build_compiler.js",
        "test": "mocha"
    },
    "version": "20170218.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module google-closure-compiler](#apidoc.module.google-closure-compiler)
1.  [function <span class="apidocSignatureSpan">google-closure-compiler.</span>compiler (args, extraCommandArgs)](#apidoc.element.google-closure-compiler.compiler)
1.  [function <span class="apidocSignatureSpan">google-closure-compiler.</span>grunt (grunt, extraArguments)](#apidoc.element.google-closure-compiler.grunt)
1.  [function <span class="apidocSignatureSpan">google-closure-compiler.</span>gulp (initOptions)](#apidoc.element.google-closure-compiler.gulp)
1.  object <span class="apidocSignatureSpan">google-closure-compiler.</span>compiler.prototype

#### [module google-closure-compiler.compiler](#apidoc.module.google-closure-compiler.compiler)
1.  [function <span class="apidocSignatureSpan">google-closure-compiler.</span>compiler (args, extraCommandArgs)](#apidoc.element.google-closure-compiler.compiler.compiler)
1.  string <span class="apidocSignatureSpan">google-closure-compiler.compiler.</span>COMPILER_PATH
1.  string <span class="apidocSignatureSpan">google-closure-compiler.compiler.</span>CONTRIB_PATH
1.  string <span class="apidocSignatureSpan">google-closure-compiler.compiler.</span>JAR_PATH

#### [module google-closure-compiler.compiler.prototype](#apidoc.module.google-closure-compiler.compiler.prototype)
1.  [function <span class="apidocSignatureSpan">google-closure-compiler.compiler.prototype.</span>formatArgument (key, val)](#apidoc.element.google-closure-compiler.compiler.prototype.formatArgument)
1.  [function <span class="apidocSignatureSpan">google-closure-compiler.compiler.prototype.</span>getFullCommand ()](#apidoc.element.google-closure-compiler.compiler.prototype.getFullCommand)
1.  [function <span class="apidocSignatureSpan">google-closure-compiler.compiler.prototype.</span>prependFullCommand (msg)](#apidoc.element.google-closure-compiler.compiler.prototype.prependFullCommand)
1.  [function <span class="apidocSignatureSpan">google-closure-compiler.compiler.prototype.</span>run (callback)](#apidoc.element.google-closure-compiler.compiler.prototype.run)
1.  object <span class="apidocSignatureSpan">google-closure-compiler.compiler.prototype.</span>logger
1.  string <span class="apidocSignatureSpan">google-closure-compiler.compiler.prototype.</span>javaPath



# <a name="apidoc.module.google-closure-compiler"></a>[module google-closure-compiler](#apidoc.module.google-closure-compiler)

#### <a name="apidoc.element.google-closure-compiler.compiler"></a>[function <span class="apidocSignatureSpan">google-closure-compiler.</span>compiler (args, extraCommandArgs)](#apidoc.element.google-closure-compiler.compiler)
- description and source-code
```javascript
function Compiler(args, extraCommandArgs) {
  this.commandArguments = (extraCommandArgs || []).slice();

  if (Compiler.JAR_PATH) {
    this.commandArguments.push('-jar', Compiler.JAR_PATH);
  }

  if (Array.isArray(args)) {
    this.commandArguments = this.commandArguments.concat(args.slice());
  } else {
    for (var key in args) {
      if (Array.isArray(args[key])) {
        for (var i = 0; i < args[key].length; i++) {
          this.commandArguments.push(
              this.formatArgument(key, args[key][i]));
        }
      } else {
        this.commandArguments.push(
            this.formatArgument(key, args[key]));
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-closure-compiler.grunt"></a>[function <span class="apidocSignatureSpan">google-closure-compiler.</span>grunt (grunt, extraArguments)](#apidoc.element.google-closure-compiler.grunt)
- description and source-code
```javascript
grunt = function (grunt, extraArguments) {
  var chalk = require('chalk');
  var VinylStream = require('./vinyl-stream');
  var fs = require('fs');
  var path = require('path');
  var gulpCompiler = require('../gulp')({extraArguments: extraArguments});
  var Transform = require('stream').Transform;
  var gulpCompilerOptions = {
    streamMode: 'IN',
    logger: grunt.log,
    pluginName: 'grunt-google-closure-compiler',
    requireStreamInput: false
  };

<span class="apidocCodeCommentSpan">  /**
   * @param {Array<string>}|null} files
   * @param {Object<string,string|boolean|Array<string>>|Array<string>} options
   * @return {Promise}
   */
</span>  function compilationPromise(files, options) {
    var hadError = false;
    function logFile(cb) {
      // If an error was encoutered, it will have already been logged
      if (!hadError) {
        if (options.js_output_file) {
          grunt.log.ok(chalk.cyan(options.js_output_file) + ' created');
        } else {
          grunt.log.ok('Compilation succeeded');
        }
      }
      cb();
    }

    var loggingStream = new Transform({
      objectMode: true,
      transform: function() {},
      flush: logFile
    });

    return new Promise(function(resolve, reject) {
      var stream;
      if (files) {
        // Source files were provided by grunt. Read these
        // in to a stream of vinyl files and pipe them through
        // the compiler task
        stream = new VinylStream(files, {base: process.cwd()})
            .pipe(gulpCompiler(options, gulpCompilerOptions));
      } else {
        // No source files were provided. Assume the options specify
        // --js flags and invoke the compiler without any grunt inputs.
        // Manually end the stream to force compilation to begin.
        stream = gulpCompiler(options, gulpCompilerOptions);
        stream.end();
      }

      stream.on('error', function(err) {
        hadError = true;
        reject(err);
      });
      stream.on('end', function(err) {
        resolve();
      });

      stream.pipe(loggingStream);
      stream.resume(); //logging stream doesn't output files, so we have to manually resume;
    });
  }

  function closureCompilerGruntTask() {
    var taskObject = this;
    var asyncDone = this.async();
    var compileTasks = [];

    function getCompilerOptions() {
      var opts = taskObject.options({
        args: undefined
      });

      var args = opts.args;

      delete opts.args;

      return {
        args: args,
        compilerOpts: opts
      }
    }

    // Invoke the compiler once for each set of source files
    taskObject.files.forEach(function (f) {
      var options = getCompilerOptions();

      var src = f.src.filter(function (filepath) {
        if (!grunt.file.exists(filepath)) {
          grunt.log.warn('Source file ' + chalk.cyan(filepath) + ' not found');
          return false;
        }
        return true;
      });

      // Require source files
      if (src.length === 0) {
        grunt.log.warn('Destination ' + chalk.cyan(f.dest) +
            ' not written because src files were empty');
        return;
      } else {
        options.compilerOpts.js_output_file = f.dest;
      }

      compileTasks.push(compilationPromise(src, options.args || options.compilerOpts)
          .then(function () {}, function(err) {
            throw err;
          }));
    });

    // If the task was invoked without any files provided by grunt, assume that
    // --js flags are present and we want to run the compiler anyway.
    if (taskObject.files.length === 0) {
      var options = getCompilerOptions();
      compileTasks.push(compilationPromise(null, options.args || options.compilerOpts));
    }

    // Multiple invocations of the compiler can occur for a single task target. Wait until
    // they are all completed before calling the "done" method.
    Promise.all(compileTasks).then(function () {
      asyncDone();
    }, function () {
      grunt.fail.warn('Compilation error');
      asyncDone();
    });
  }

  grunt.registerMultiTask('closure-compiler',
      'Minify files with Google Closure Compiler',
      closur ...
```
- example usage
```shell
...
'''

## Using the Grunt Task

Include the plugin in your Gruntfile.js:

'''js
require('google-closure-compiler').grunt(grunt);
// The load-grunt-tasks plugin won't automatically load closure-compiler
'''

Task targets, files and options may be specified according to the grunt
[Configuring tasks](http://gruntjs.com/configuring-tasks) guide.

### Basic Configuration Example:
...
```

#### <a name="apidoc.element.google-closure-compiler.gulp"></a>[function <span class="apidocSignatureSpan">google-closure-compiler.</span>gulp (initOptions)](#apidoc.element.google-closure-compiler.gulp)
- description and source-code
```javascript
gulp = function (initOptions) {
  var filesToJson = require('./concat-to-json');
  var jsonToVinyl = require('./json-to-vinyl');
  var Compiler = require('../node/closure-compiler');
  var stream = require('stream');
<span class="apidocCodeCommentSpan">  /** @const */
</span>  var PLUGIN_NAME = 'gulp-google-closure-compiler';

  var extraCommandArguments = initOptions ? initOptions.extraArguments : undefined;
  var applySourceMap = require('vinyl-sourcemaps-apply');
  var path = require('path');
  var chalk = require('chalk');
  var File = require('vinyl');

  /** @constructor */
  function CustomError(plugin, msg) {
    var superError = Error.call(this) || this;
    Error.captureStackTrace(superError, this.constructor);
    superError.name = 'Error';
    superError.message = msg;
    return superError;
  }
  CustomError.prototype = Object.create(Error.prototype);
  CustomError.prototype.name = 'Error';

  var PluginError;
  try {
    PluginError = require('gulp-util').PluginError;
  } catch(e) {
    PluginError = CustomError;
  }

  var gulpLog;
  try {
    gulpLog = require('gulp-util').log;
  } catch(e) {
    gulpLog = console;
  }

  function CompilationStream(compilationOptions, pluginOptions) {
    stream.Transform.call(this, {objectMode: true});

    pluginOptions = pluginOptions || {};

    this.compilatonOptions_ = compilationOptions;
    this.streamMode_ = pluginOptions.streamMode || 'BOTH';
    this.logger_ = pluginOptions.logger || gulpLog;
    this.PLUGIN_NAME_ = pluginOptions.pluginName || PLUGIN_NAME;

    this.fileList_ = [];
    this._streamInputRequired = pluginOptions.requireStreamInput !== false;
  }
  CompilationStream.prototype = Object.create(stream.Transform.prototype);

  // Buffer the files into an array
  CompilationStream.prototype.src = function() {
    this._streamInputRequired = false;
    process.nextTick((function() {
      var stdInStream = new stream.Readable({ read: function() {
        return new File();
      }});
      stdInStream.pipe(this);
      stdInStream.push(null);
    }).bind(this));
    return this;
  };

  // Buffer the files into an array
  CompilationStream.prototype._transform = function(file, enc, cb) {
    // ignore empty files
    if (file.isNull()) {
      cb();
      return;
    }

    if (file.isStream()) {
      this.emit('error', new PluginError(this.PLUGIN_NAME_, 'Streaming not supported'));
      cb();
      return;
    }

    this.fileList_.push(file);
    cb();
  };

  CompilationStream.prototype._flush = function(cb) {
    var jsonFiles, logger = this.logger_.warn ? this.logger_.warn : this.logger_;
    if (this.fileList_.length > 0) {
      // Input files are present. Convert them to a JSON encoded string
      jsonFiles = filesToJson(this.fileList_);
    } else {
      // If files in the stream were required, no compilation needed here.
      if (this._streamInputRequired) {
        this.emit('end');
        cb();
        return;
      }

      // The compiler will always expect something on standard-in. So pass it an empty
      // list if no files were piped into this plugin.
      jsonFiles = [];
    }

    var compiler = new Compiler(this.compilatonOptions_, extraCommandArguments);

    // Add the gulp-specific argument so the compiler will understand the JSON encoded input
    // for gulp, the stream mode will be 'BOTH', but when invoked from grunt, we only use
    // a stream mode of 'IN'
    compiler.commandArguments.push('--json_streams', this.streamMode_);

    var compilerProcess = compiler.run();

    var stdOutData = '', stdErrData = '';

    compilerProcess.stdout.on('data', function (data) {
      stdOutData += data;
    });
    compilerProcess.stderr.on('data', function (data) {
      stdErrData += data;
    });

    Promise.all([
      new Promise(function(resolve) {
        compilerProcess.on('close', function(code) {
          resolve(code);
        });
      }),
      new Promise(function(resolve) {
        compilerProcess.stdout.on('end', function() {
          resolve();
        });
      }),
      new Promise(function(resolve) {
        compilerProcess.stderr.on('end', function() { ...
```
- example usage
```shell
...
The gulp plugin supports piping multiple files through the compiler.

Options are a direct match to the compiler flags without the leading "--".

### Basic Configuration Example:

'''js
var closureCompiler = require('google-closure-compiler').gulp();

gulp.task('js-compile', function () {
return gulp.src('./src/js/**/*.js', {base: './'})
    .pipe(closureCompiler({
        compilation_level: 'SIMPLE',
        warning_level: 'VERBOSE',
        language_in: 'ECMASCRIPT6_STRICT',
...
```



# <a name="apidoc.module.google-closure-compiler.compiler"></a>[module google-closure-compiler.compiler](#apidoc.module.google-closure-compiler.compiler)

#### <a name="apidoc.element.google-closure-compiler.compiler.compiler"></a>[function <span class="apidocSignatureSpan">google-closure-compiler.</span>compiler (args, extraCommandArgs)](#apidoc.element.google-closure-compiler.compiler.compiler)
- description and source-code
```javascript
function Compiler(args, extraCommandArgs) {
  this.commandArguments = (extraCommandArgs || []).slice();

  if (Compiler.JAR_PATH) {
    this.commandArguments.push('-jar', Compiler.JAR_PATH);
  }

  if (Array.isArray(args)) {
    this.commandArguments = this.commandArguments.concat(args.slice());
  } else {
    for (var key in args) {
      if (Array.isArray(args[key])) {
        for (var i = 0; i < args[key].length; i++) {
          this.commandArguments.push(
              this.formatArgument(key, args[key][i]));
        }
      } else {
        this.commandArguments.push(
            this.formatArgument(key, args[key]));
      }
    }
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.google-closure-compiler.compiler.prototype"></a>[module google-closure-compiler.compiler.prototype](#apidoc.module.google-closure-compiler.compiler.prototype)

#### <a name="apidoc.element.google-closure-compiler.compiler.prototype.formatArgument"></a>[function <span class="apidocSignatureSpan">google-closure-compiler.compiler.prototype.</span>formatArgument (key, val)](#apidoc.element.google-closure-compiler.compiler.prototype.formatArgument)
- description and source-code
```javascript
formatArgument = function (key, val) {
  if (val === undefined || val === null) {
    return '--' + key;
  }

  return '--' + key + '=' + val;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-closure-compiler.compiler.prototype.getFullCommand"></a>[function <span class="apidocSignatureSpan">google-closure-compiler.compiler.prototype.</span>getFullCommand ()](#apidoc.element.google-closure-compiler.compiler.prototype.getFullCommand)
- description and source-code
```javascript
getFullCommand = function () {
  return this.javaPath + ' ' + this.commandArguments.join(' ');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-closure-compiler.compiler.prototype.prependFullCommand"></a>[function <span class="apidocSignatureSpan">google-closure-compiler.compiler.prototype.</span>prependFullCommand (msg)](#apidoc.element.google-closure-compiler.compiler.prototype.prependFullCommand)
- description and source-code
```javascript
prependFullCommand = function (msg) {
  return this.getFullCommand() + '\n\n' + msg + '\n\n';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.google-closure-compiler.compiler.prototype.run"></a>[function <span class="apidocSignatureSpan">google-closure-compiler.compiler.prototype.</span>run (callback)](#apidoc.element.google-closure-compiler.compiler.prototype.run)
- description and source-code
```javascript
run = function (callback) {
  if (this.logger) {
    this.logger(this.getFullCommand() + '\n');
  }

  var compileProcess = spawn(this.javaPath, this.commandArguments, this.spawnOptions);

  var stdOutData = '', stdErrData = '';
  if (callback) {
    compileProcess.stdout.on('data', function (data) {
      stdOutData += data;
    });

    compileProcess.stderr.on('data', function (data) {
      stdErrData += data;
    });

    compileProcess.on('close', (function (code) {
      if (code !== 0) {
        stdErrData = this.prependFullCommand(stdErrData);
      }

      callback(code, stdOutData, stdErrData);
    }).bind(this));

    compileProcess.on('error', (function (err) {
      callback(1, stdOutData,
          this.prependFullCommand('Process spawn error. Is java in the path?\n' + err.message));
    }).bind(this));
  }

  return compileProcess;
}
```
- example usage
```shell
...
console.log(ClosureCompiler.CONTRIB_PATH); // absolute path the contrib folder which contains

var closureCompiler = new ClosureCompiler({
  js: 'file-one.js',
  compilation_level: 'ADVANCED'
});

var compilerProcess = closureCompiler.run(function(exitCode, stdOut, stdErr) {
  //compilation complete
});
'''

## License
Copyright 2015 The Closure Compiler Authors
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
