# api documentation for  [js-yaml (v3.8.2)](https://github.com/nodeca/js-yaml)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-js-yaml.svg)](https://travis-ci.org/npmdoc/node-npmdoc-js-yaml)
#### YAML 1.2 parser and serializer

[![NPM](https://nodei.co/npm/js-yaml.png?downloads=true)](https://www.npmjs.com/package/js-yaml)

[![apidoc](https://npmdoc.github.io/node-npmdoc-js-yaml/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-js_yaml_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-js-yaml/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-js-yaml/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Vladimir Zapparov",
        "email": "dervus.grim@gmail.com"
    },
    "bin": {
        "js-yaml": "bin/js-yaml.js"
    },
    "bugs": {
        "url": "https://github.com/nodeca/js-yaml/issues"
    },
    "contributors": [
        {
            "name": "Aleksey V Zapparov",
            "email": "ixti@member.fsf.org",
            "url": "http://www.ixti.net/"
        },
        {
            "name": "Vitaly Puzrin",
            "email": "vitaly@rcdesign.ru",
            "url": "https://github.com/puzrin"
        },
        {
            "name": "Martin Grenfell",
            "email": "martin.grenfell@gmail.com",
            "url": "http://got-ravings.blogspot.com"
        }
    ],
    "dependencies": {
        "argparse": "^1.0.7",
        "esprima": "^3.1.1"
    },
    "description": "YAML 1.2 parser and serializer",
    "devDependencies": {
        "ansi": "*",
        "benchmark": "*",
        "browserify": "^13.0.0",
        "codemirror": "^5.13.4",
        "eslint": "^3.10.0",
        "istanbul": "*",
        "mocha": "*",
        "uglify-js": "^2.6.1"
    },
    "directories": {},
    "dist": {
        "shasum": "02d3e2c0f6beab20248d412c352203827d786721",
        "tarball": "https://registry.npmjs.org/js-yaml/-/js-yaml-3.8.2.tgz"
    },
    "files": [
        "index.js",
        "lib/",
        "bin/",
        "dist/"
    ],
    "gitHead": "7dd7254139804a0cd15683fd9e61ad949bd5ce14",
    "homepage": "https://github.com/nodeca/js-yaml",
    "keywords": [
        "yaml",
        "parser",
        "serializer",
        "pyyaml"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "vitaly",
            "email": "vitaly@rcdesign.ru"
        }
    ],
    "name": "js-yaml",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/nodeca/js-yaml.git"
    },
    "scripts": {
        "test": "make test"
    },
    "version": "3.8.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module js-yaml](#apidoc.module.js-yaml)
1.  [function <span class="apidocSignatureSpan">js-yaml.</span>Schema (definition)](#apidoc.element.js-yaml.Schema)
1.  [function <span class="apidocSignatureSpan">js-yaml.</span>Type (tag, options)](#apidoc.element.js-yaml.Type)
1.  [function <span class="apidocSignatureSpan">js-yaml.</span>YAMLException (reason, mark)](#apidoc.element.js-yaml.YAMLException)
1.  [function <span class="apidocSignatureSpan">js-yaml.</span>addConstructor ()](#apidoc.element.js-yaml.addConstructor)
1.  [function <span class="apidocSignatureSpan">js-yaml.</span>compose ()](#apidoc.element.js-yaml.compose)
1.  [function <span class="apidocSignatureSpan">js-yaml.</span>dump (input, options)](#apidoc.element.js-yaml.dump)
1.  [function <span class="apidocSignatureSpan">js-yaml.</span>load (input, options)](#apidoc.element.js-yaml.load)
1.  [function <span class="apidocSignatureSpan">js-yaml.</span>loadAll (input, iterator, options)](#apidoc.element.js-yaml.loadAll)
1.  [function <span class="apidocSignatureSpan">js-yaml.</span>parse ()](#apidoc.element.js-yaml.parse)
1.  [function <span class="apidocSignatureSpan">js-yaml.</span>safeDump (input, options)](#apidoc.element.js-yaml.safeDump)
1.  [function <span class="apidocSignatureSpan">js-yaml.</span>safeLoad (input, options)](#apidoc.element.js-yaml.safeLoad)
1.  [function <span class="apidocSignatureSpan">js-yaml.</span>safeLoadAll (input, output, options)](#apidoc.element.js-yaml.safeLoadAll)
1.  [function <span class="apidocSignatureSpan">js-yaml.</span>scan ()](#apidoc.element.js-yaml.scan)
1.  object <span class="apidocSignatureSpan">js-yaml.</span>CORE_SCHEMA
1.  object <span class="apidocSignatureSpan">js-yaml.</span>DEFAULT_FULL_SCHEMA
1.  object <span class="apidocSignatureSpan">js-yaml.</span>DEFAULT_SAFE_SCHEMA
1.  object <span class="apidocSignatureSpan">js-yaml.</span>DEFAULT_SCHEMA
1.  object <span class="apidocSignatureSpan">js-yaml.</span>FAILSAFE_SCHEMA
1.  object <span class="apidocSignatureSpan">js-yaml.</span>JSON_SCHEMA
1.  object <span class="apidocSignatureSpan">js-yaml.</span>MINIMAL_SCHEMA
1.  object <span class="apidocSignatureSpan">js-yaml.</span>SAFE_SCHEMA
1.  object <span class="apidocSignatureSpan">js-yaml.</span>YAMLException.prototype

#### [module js-yaml.Schema](#apidoc.module.js-yaml.Schema)
1.  [function <span class="apidocSignatureSpan">js-yaml.</span>Schema (definition)](#apidoc.element.js-yaml.Schema.Schema)
1.  [function <span class="apidocSignatureSpan">js-yaml.Schema.</span>create ()](#apidoc.element.js-yaml.Schema.create)
1.  object <span class="apidocSignatureSpan">js-yaml.Schema.</span>DEFAULT

#### [module js-yaml.YAMLException](#apidoc.module.js-yaml.YAMLException)
1.  [function <span class="apidocSignatureSpan">js-yaml.</span>YAMLException (reason, mark)](#apidoc.element.js-yaml.YAMLException.YAMLException)

#### [module js-yaml.YAMLException.prototype](#apidoc.module.js-yaml.YAMLException.prototype)
1.  [function <span class="apidocSignatureSpan">js-yaml.YAMLException.prototype.</span>constructor (reason, mark)](#apidoc.element.js-yaml.YAMLException.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">js-yaml.YAMLException.prototype.</span>toString (compact)](#apidoc.element.js-yaml.YAMLException.prototype.toString)



# <a name="apidoc.module.js-yaml"></a>[module js-yaml](#apidoc.module.js-yaml)

#### <a name="apidoc.element.js-yaml.Schema"></a>[function <span class="apidocSignatureSpan">js-yaml.</span>Schema (definition)](#apidoc.element.js-yaml.Schema)
- description and source-code
```javascript
function Schema(definition) {
  this.include  = definition.include  || [];
  this.implicit = definition.implicit || [];
  this.explicit = definition.explicit || [];

  this.implicit.forEach(function (type) {
    if (type.loadKind && type.loadKind !== 'scalar') {
      throw new YAMLException('There is a non-scalar type in the implicit list of a schema. Implicit resolving of such types is
not supported.');
    }
  });

  this.compiledImplicit = compileList(this, 'implicit', []);
  this.compiledExplicit = compileList(this, 'explicit', []);
  this.compiledTypeMap  = compileMap(this.compiledImplicit, this.compiledExplicit);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-yaml.Type"></a>[function <span class="apidocSignatureSpan">js-yaml.</span>Type (tag, options)](#apidoc.element.js-yaml.Type)
- description and source-code
```javascript
function Type(tag, options) {
  options = options || {};

  Object.keys(options).forEach(function (name) {
    if (TYPE_CONSTRUCTOR_OPTIONS.indexOf(name) === -1) {
      throw new YAMLException('Unknown option "' + name + '" is met in definition of "' + tag + '" YAML type.');
    }
  });

  // TODO: Add tag format check.
  this.tag          = tag;
  this.kind         = options['kind']         || null;
  this.resolve      = options['resolve']      || function () { return true; };
  this.construct    = options['construct']    || function (data) { return data; };
  this.instanceOf   = options['instanceOf']   || null;
  this.predicate    = options['predicate']    || null;
  this.represent    = options['represent']    || null;
  this.defaultStyle = options['defaultStyle'] || null;
  this.styleAliases = compileStyleAliases(options['styleAliases'] || null);

  if (YAML_NODE_KINDS.indexOf(this.kind) === -1) {
    throw new YAMLException('Unknown kind "' + this.kind + '" is specified for "' + tag + '" YAML type.');
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-yaml.YAMLException"></a>[function <span class="apidocSignatureSpan">js-yaml.</span>YAMLException (reason, mark)](#apidoc.element.js-yaml.YAMLException)
- description and source-code
```javascript
function YAMLException(reason, mark) {
  // Super constructor
  Error.call(this);

  // Include stack trace in error object
  if (Error.captureStackTrace) {
    // Chrome and NodeJS
    Error.captureStackTrace(this, this.constructor);
  } else {
    // FF, IE 10+ and Safari 6+. Fallback for others
    this.stack = (new Error()).stack || '';
  }

  this.name = 'YAMLException';
  this.reason = reason;
  this.mark = mark;
  this.message = (this.reason || '(unknown reason)') + (this.mark ? ' ' + this.mark.toString() : '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-yaml.addConstructor"></a>[function <span class="apidocSignatureSpan">js-yaml.</span>addConstructor ()](#apidoc.element.js-yaml.addConstructor)
- description and source-code
```javascript
addConstructor = function () {
  throw new Error('Function ' + name + ' is deprecated and cannot be used.');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-yaml.compose"></a>[function <span class="apidocSignatureSpan">js-yaml.</span>compose ()](#apidoc.element.js-yaml.compose)
- description and source-code
```javascript
compose = function () {
  throw new Error('Function ' + name + ' is deprecated and cannot be used.');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-yaml.dump"></a>[function <span class="apidocSignatureSpan">js-yaml.</span>dump (input, options)](#apidoc.element.js-yaml.dump)
- description and source-code
```javascript
function dump(input, options) {
  options = options || {};

  var state = new State(options);

  if (!state.noRefs) getDuplicateReferences(input, state);

  if (writeNode(state, 0, input, true, true)) return state.dump + '\n';

  return '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-yaml.load"></a>[function <span class="apidocSignatureSpan">js-yaml.</span>load (input, options)](#apidoc.element.js-yaml.load)
- description and source-code
```javascript
function load(input, options) {
  var documents = loadDocuments(input, options);

  if (documents.length === 0) {
<span class="apidocCodeCommentSpan">    /*eslint-disable no-undefined*/
</span>    return undefined;
  } else if (documents.length === 1) {
    return documents[0];
  }
  throw new YAMLException('expected a single document in the stream, but found more');
}
```
- example usage
```shell
...
### Bundled YAML library for browsers

''' html
<!-- esprima required only for !!js/function -->
<script src="esprima.js"></script>
<script src="js-yaml.min.js"></script>
<script type="text/javascript">
var doc = jsyaml.load('greeting: hello\nname: world');
</script>
'''

Browser support was done mostly for online demo. If you find any errors - feel
free to send pull requests with fixes. Also note, that IE and other old browsers
needs [es5-shims](https://github.com/kriskowal/es5-shim) to operate.
...
```

#### <a name="apidoc.element.js-yaml.loadAll"></a>[function <span class="apidocSignatureSpan">js-yaml.</span>loadAll (input, iterator, options)](#apidoc.element.js-yaml.loadAll)
- description and source-code
```javascript
function loadAll(input, iterator, options) {
  var documents = loadDocuments(input, options), index, length;

  for (index = 0, length = documents.length; index < length; index += 1) {
    iterator(documents[index]);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-yaml.parse"></a>[function <span class="apidocSignatureSpan">js-yaml.</span>parse ()](#apidoc.element.js-yaml.parse)
- description and source-code
```javascript
parse = function () {
  throw new Error('Function ' + name + ' is deprecated and cannot be used.');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-yaml.safeDump"></a>[function <span class="apidocSignatureSpan">js-yaml.</span>safeDump (input, options)](#apidoc.element.js-yaml.safeDump)
- description and source-code
```javascript
function safeDump(input, options) {
  return dump(input, common.extend({ schema: DEFAULT_SAFE_SCHEMA }, options));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-yaml.safeLoad"></a>[function <span class="apidocSignatureSpan">js-yaml.</span>safeLoad (input, options)](#apidoc.element.js-yaml.safeLoad)
- description and source-code
```javascript
function safeLoad(input, options) {
  return load(input, common.extend({ schema: DEFAULT_SAFE_SCHEMA }, options));
}
```
- example usage
```shell
...

''' javascript
yaml = require('js-yaml');
fs   = require('fs');

// Get document, or throw exception on error
try {
  var doc = yaml.safeLoad(fs.readFileSync('/home/ixti/example.yml', 'utf8'));
  console.log(doc);
} catch (e) {
  console.log(e);
}
'''
...
```

#### <a name="apidoc.element.js-yaml.safeLoadAll"></a>[function <span class="apidocSignatureSpan">js-yaml.</span>safeLoadAll (input, output, options)](#apidoc.element.js-yaml.safeLoadAll)
- description and source-code
```javascript
function safeLoadAll(input, output, options) {
  loadAll(input, output, common.extend({ schema: DEFAULT_SAFE_SCHEMA }, options));
}
```
- example usage
```shell
...

Same as 'safeLoad()', but understands multi-document sources and apply
'iterator' to each document.

''' javascript
var yaml = require('js-yaml');

yaml.safeLoadAll(data, function (doc) {
  console.log(doc);
});
'''


### loadAll (string, iterator [ , options ])
...
```

#### <a name="apidoc.element.js-yaml.scan"></a>[function <span class="apidocSignatureSpan">js-yaml.</span>scan ()](#apidoc.element.js-yaml.scan)
- description and source-code
```javascript
scan = function () {
  throw new Error('Function ' + name + ' is deprecated and cannot be used.');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.js-yaml.Schema"></a>[module js-yaml.Schema](#apidoc.module.js-yaml.Schema)

#### <a name="apidoc.element.js-yaml.Schema.Schema"></a>[function <span class="apidocSignatureSpan">js-yaml.</span>Schema (definition)](#apidoc.element.js-yaml.Schema.Schema)
- description and source-code
```javascript
function Schema(definition) {
  this.include  = definition.include  || [];
  this.implicit = definition.implicit || [];
  this.explicit = definition.explicit || [];

  this.implicit.forEach(function (type) {
    if (type.loadKind && type.loadKind !== 'scalar') {
      throw new YAMLException('There is a non-scalar type in the implicit list of a schema. Implicit resolving of such types is
not supported.');
    }
  });

  this.compiledImplicit = compileList(this, 'implicit', []);
  this.compiledExplicit = compileList(this, 'explicit', []);
  this.compiledTypeMap  = compileMap(this.compiledImplicit, this.compiledExplicit);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-yaml.Schema.create"></a>[function <span class="apidocSignatureSpan">js-yaml.Schema.</span>create ()](#apidoc.element.js-yaml.Schema.create)
- description and source-code
```javascript
function createSchema() {
  var schemas, types;

  switch (arguments.length) {
    case 1:
      schemas = Schema.DEFAULT;
      types = arguments[0];
      break;

    case 2:
      schemas = arguments[0];
      types = arguments[1];
      break;

    default:
      throw new YAMLException('Wrong number of arguments for Schema.create function');
  }

  schemas = common.toArray(schemas);
  types = common.toArray(types);

  if (!schemas.every(function (schema) { return schema instanceof Schema; })) {
    throw new YAMLException('Specified list of super schemas (or a single Schema object) contains a non-Schema object.');
  }

  if (!types.every(function (type) { return type instanceof Type; })) {
    throw new YAMLException('Specified list of YAML types (or a single Type object) contains a non-Type object.');
  }

  return new Schema({
    include: schemas,
    explicit: types
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.js-yaml.YAMLException"></a>[module js-yaml.YAMLException](#apidoc.module.js-yaml.YAMLException)

#### <a name="apidoc.element.js-yaml.YAMLException.YAMLException"></a>[function <span class="apidocSignatureSpan">js-yaml.</span>YAMLException (reason, mark)](#apidoc.element.js-yaml.YAMLException.YAMLException)
- description and source-code
```javascript
function YAMLException(reason, mark) {
  // Super constructor
  Error.call(this);

  // Include stack trace in error object
  if (Error.captureStackTrace) {
    // Chrome and NodeJS
    Error.captureStackTrace(this, this.constructor);
  } else {
    // FF, IE 10+ and Safari 6+. Fallback for others
    this.stack = (new Error()).stack || '';
  }

  this.name = 'YAMLException';
  this.reason = reason;
  this.mark = mark;
  this.message = (this.reason || '(unknown reason)') + (this.mark ? ' ' + this.mark.toString() : '');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.js-yaml.YAMLException.prototype"></a>[module js-yaml.YAMLException.prototype](#apidoc.module.js-yaml.YAMLException.prototype)

#### <a name="apidoc.element.js-yaml.YAMLException.prototype.constructor"></a>[function <span class="apidocSignatureSpan">js-yaml.YAMLException.prototype.</span>constructor (reason, mark)](#apidoc.element.js-yaml.YAMLException.prototype.constructor)
- description and source-code
```javascript
function YAMLException(reason, mark) {
  // Super constructor
  Error.call(this);

  // Include stack trace in error object
  if (Error.captureStackTrace) {
    // Chrome and NodeJS
    Error.captureStackTrace(this, this.constructor);
  } else {
    // FF, IE 10+ and Safari 6+. Fallback for others
    this.stack = (new Error()).stack || '';
  }

  this.name = 'YAMLException';
  this.reason = reason;
  this.mark = mark;
  this.message = (this.reason || '(unknown reason)') + (this.mark ? ' ' + this.mark.toString() : '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.js-yaml.YAMLException.prototype.toString"></a>[function <span class="apidocSignatureSpan">js-yaml.YAMLException.prototype.</span>toString (compact)](#apidoc.element.js-yaml.YAMLException.prototype.toString)
- description and source-code
```javascript
function toString(compact) {
  var result = this.name + ': ';

  result += this.reason || '(unknown reason)';

  if (!compact && this.mark) {
    result += ' ' + this.mark.toString();
  }

  return result;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
