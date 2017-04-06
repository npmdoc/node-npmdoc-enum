# api documentation for  [enum (v2.4.0)](https://github.com/adrai/enum)  [![npm package](https://img.shields.io/npm/v/npmdoc-enum.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-enum) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-enum.svg)](https://travis-ci.org/npmdoc/node-npmdoc-enum)
#### Enum is a javascript module that introduces the Enum Type. It works for node.js and in the browser.

[![NPM](https://nodei.co/npm/enum.png?downloads=true)](https://www.npmjs.com/package/enum)

[![apidoc](https://npmdoc.github.io/node-npmdoc-enum/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-enum_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-enum/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-enum/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-enum/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "adrai"
    },
    "bugs": {
        "url": "https://github.com/adrai/enum/issues"
    },
    "dependencies": {
        "is-buffer": "^1.1.0"
    },
    "description": "Enum is a javascript module that introduces the Enum Type. It works for node.js and in the browser.",
    "devDependencies": {
        "expect.js": ">= 0.1.2",
        "gulp": "^3.8.11",
        "gulp-babel": "^4.0.0",
        "gulp-bench": "^1.1.0",
        "gulp-browserify": "^0.5.1",
        "gulp-mocha": "^2.0.0",
        "gulp-rename": "^1.2.0",
        "gulp-rimraf": "^0.1.1",
        "gulp-shell": "^0.4.0",
        "gulp-uglify": "^1.1.0",
        "mocha": ">= 1.0.1",
        "zuul": ">= 1.0.1"
    },
    "directories": {
        "lib": "./lib"
    },
    "dist": {
        "shasum": "1aea67cdf74a34e6d8198283b2b3cb348e221b5e",
        "tarball": "https://registry.npmjs.org/enum/-/enum-2.4.0.tgz"
    },
    "engines": {
        "node": ">=0.6.0"
    },
    "gitHead": "ef3b6f8b5f3e306ef315ca1d794f7b2725131192",
    "homepage": "https://github.com/adrai/enum",
    "keywords": [
        "enum"
    ],
    "licenses": [
        {
            "type": "MIT",
            "url": "https://raw.github.com/adrai/enum/master/licence"
        }
    ],
    "main": "index.js",
    "maintainers": [
        {
            "name": "adrai",
            "email": "adriano@raiano.ch"
        },
        {
            "name": "schtoeffel",
            "email": "schtoeffel@gmail.com"
        }
    ],
    "name": "enum",
    "optionalDependencies": {},
    "private": false,
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/adrai/enum.git"
    },
    "scripts": {
        "build": "gulp build",
        "prepublish": "gulp",
        "test": "gulp test-ci"
    },
    "testling": {
        "browsers": [
            "ie/6..latest",
            "firefox/17..latest",
            "firefox/nightly",
            "chrome/22..latest",
            "chrome/canary",
            "opera/12..latest",
            "opera/next",
            "safari/5.1..latest",
            "ipad/6.0..latest",
            "iphone/6.0..latest",
            "android-browser/4.2..latest"
        ],
        "harness": "mocha",
        "files": "test/*.js"
    },
    "version": "2.4.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module enum](#apidoc.module.enum)
1.  [function <span class="apidocSignatureSpan">enum.</span>enum_2_4_0 (map, options)](#apidoc.element.enum.enum_2_4_0)
1.  [function <span class="apidocSignatureSpan">enum.</span>register ()](#apidoc.element.enum.register)
1.  object <span class="apidocSignatureSpan">enum.</span>enum_2_4_0.prototype

#### [module enum.enum_2_4_0](#apidoc.module.enum.enum_2_4_0)
1.  [function <span class="apidocSignatureSpan">enum.</span>enum_2_4_0 (map, options)](#apidoc.element.enum.enum_2_4_0.enum_2_4_0)
1.  [function <span class="apidocSignatureSpan">enum.enum_2_4_0.</span>register ()](#apidoc.element.enum.enum_2_4_0.register)

#### [module enum.enum_2_4_0.prototype](#apidoc.module.enum.enum_2_4_0.prototype)
1.  [function <span class="apidocSignatureSpan">enum.enum_2_4_0.prototype.</span>extend (map)](#apidoc.element.enum.enum_2_4_0.prototype.extend)
1.  [function <span class="apidocSignatureSpan">enum.enum_2_4_0.prototype.</span>freezeEnums ()](#apidoc.element.enum.enum_2_4_0.prototype.freezeEnums)
1.  [function <span class="apidocSignatureSpan">enum.enum_2_4_0.prototype.</span>get (key, offset)](#apidoc.element.enum.enum_2_4_0.prototype.get)
1.  [function <span class="apidocSignatureSpan">enum.enum_2_4_0.prototype.</span>getKey (value)](#apidoc.element.enum.enum_2_4_0.prototype.getKey)
1.  [function <span class="apidocSignatureSpan">enum.enum_2_4_0.prototype.</span>getValue (key)](#apidoc.element.enum.enum_2_4_0.prototype.getValue)
1.  [function <span class="apidocSignatureSpan">enum.enum_2_4_0.prototype.</span>isDefined (enumItem)](#apidoc.element.enum.enum_2_4_0.prototype.isDefined)
1.  [function <span class="apidocSignatureSpan">enum.enum_2_4_0.prototype.</span>set (buffer, offset, value)](#apidoc.element.enum.enum_2_4_0.prototype.set)
1.  [function <span class="apidocSignatureSpan">enum.enum_2_4_0.prototype.</span>toJSON ()](#apidoc.element.enum.enum_2_4_0.prototype.toJSON)



# <a name="apidoc.module.enum"></a>[module enum](#apidoc.module.enum)

#### <a name="apidoc.element.enum.enum_2_4_0"></a>[function <span class="apidocSignatureSpan">enum.</span>enum_2_4_0 (map, options)](#apidoc.element.enum.enum_2_4_0)
- description and source-code
```javascript
function Enum(map, options) {
  var _this = this;

  _classCallCheck(this, Enum);

<span class="apidocCodeCommentSpan">  /* implement the "ref type interface", so that Enum types can
   * be used in 'node-ffi' function declarations and invokations.
   * In C, these Enums act as 'uint32_t' types.
   *
   * https://github.com/TooTallNate/ref#the-type-interface
   */
</span>  this.size = 4;
  this.indirection = 1;

  if (options && isString(options)) {
    options = { name: options };
  }

  this._options = options || {};
  this._options.separator = this._options.separator || " | ";
  this._options.endianness = this._options.endianness || endianness;
  this._options.ignoreCase = this._options.ignoreCase || false;
  this._options.freez = this._options.freez || false;

  this.enums = [];

  if (map.length) {
    this._enumLastIndex = map.length;
    var array = map;
    map = {};

    for (var i = 0; i < array.length; i++) {
      map[array[i]] = Math.pow(2, i);
    }
  }

  for (var member in map) {
    guardReservedKeys(this._options.name, member);
    this[member] = new EnumItem(member, map[member], { ignoreCase: this._options.ignoreCase });
    this.enums.push(this[member]);
  }
  this._enumMap = map;

  if (this._options.ignoreCase) {
    this.getLowerCaseEnums = function () {
      var res = {};
      for (var i = 0, len = this.enums.length; i < len; i++) {
        res[this.enums[i].key.toLowerCase()] = this.enums[i];
      }
      return res;
    };
  }

  if (this._options.name) {
    this.name = this._options.name;
  }

  var isFlaggable = function () {
    for (var i = 0, len = _this.enums.length; i < len; i++) {
      var e = _this.enums[i];

      if (!(e.value !== 0 && !(e.value & e.value - 1))) {
        return false;
      }
    }
    return true;
  };

  this.isFlaggable = isFlaggable();
  if (this._options.freez) {
    this.freezeEnums(); //this will make instances of Enum non-extensible
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.enum.register"></a>[function <span class="apidocSignatureSpan">enum.</span>register ()](#apidoc.element.enum.register)
- description and source-code
```javascript
function register() {
  var key = arguments[0] === undefined ? "Enum" : arguments[0];

  if (!global[key]) {
    global[key] = Enum;
  }
}
```
- example usage
```shell
...
# Usage

''''js
// use it as module
var Enum = require('enum');

// or extend node.js with this new type
require('enum').register();

// define a simple enum (automatically flaggable -> A: 0x01, B: 0x02, C: 0x04)
//Uses bitwise 'OR' operation in between the values and creates enumerated constants. For example, if 'Read':1, 'Write':2, then
ReadWrite= Read | Write = 1 | 2 = 3;
var myEnum = new Enum(['A', 'B', 'C']);

//define a flagged enum object to create a multicolor option; just pass an array
var myEnum = new Enum(['Black', 'Red', 'Green', 'Blue']);
...
```



# <a name="apidoc.module.enum.enum_2_4_0"></a>[module enum.enum_2_4_0](#apidoc.module.enum.enum_2_4_0)

#### <a name="apidoc.element.enum.enum_2_4_0.enum_2_4_0"></a>[function <span class="apidocSignatureSpan">enum.</span>enum_2_4_0 (map, options)](#apidoc.element.enum.enum_2_4_0.enum_2_4_0)
- description and source-code
```javascript
function Enum(map, options) {
  var _this = this;

  _classCallCheck(this, Enum);

<span class="apidocCodeCommentSpan">  /* implement the "ref type interface", so that Enum types can
   * be used in 'node-ffi' function declarations and invokations.
   * In C, these Enums act as 'uint32_t' types.
   *
   * https://github.com/TooTallNate/ref#the-type-interface
   */
</span>  this.size = 4;
  this.indirection = 1;

  if (options && isString(options)) {
    options = { name: options };
  }

  this._options = options || {};
  this._options.separator = this._options.separator || " | ";
  this._options.endianness = this._options.endianness || endianness;
  this._options.ignoreCase = this._options.ignoreCase || false;
  this._options.freez = this._options.freez || false;

  this.enums = [];

  if (map.length) {
    this._enumLastIndex = map.length;
    var array = map;
    map = {};

    for (var i = 0; i < array.length; i++) {
      map[array[i]] = Math.pow(2, i);
    }
  }

  for (var member in map) {
    guardReservedKeys(this._options.name, member);
    this[member] = new EnumItem(member, map[member], { ignoreCase: this._options.ignoreCase });
    this.enums.push(this[member]);
  }
  this._enumMap = map;

  if (this._options.ignoreCase) {
    this.getLowerCaseEnums = function () {
      var res = {};
      for (var i = 0, len = this.enums.length; i < len; i++) {
        res[this.enums[i].key.toLowerCase()] = this.enums[i];
      }
      return res;
    };
  }

  if (this._options.name) {
    this.name = this._options.name;
  }

  var isFlaggable = function () {
    for (var i = 0, len = _this.enums.length; i < len; i++) {
      var e = _this.enums[i];

      if (!(e.value !== 0 && !(e.value & e.value - 1))) {
        return false;
      }
    }
    return true;
  };

  this.isFlaggable = isFlaggable();
  if (this._options.freez) {
    this.freezeEnums(); //this will make instances of Enum non-extensible
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.enum.enum_2_4_0.register"></a>[function <span class="apidocSignatureSpan">enum.enum_2_4_0.</span>register ()](#apidoc.element.enum.enum_2_4_0.register)
- description and source-code
```javascript
function register() {
  var key = arguments[0] === undefined ? "Enum" : arguments[0];

  if (!global[key]) {
    global[key] = Enum;
  }
}
```
- example usage
```shell
...
# Usage

''''js
// use it as module
var Enum = require('enum');

// or extend node.js with this new type
require('enum').register();

// define a simple enum (automatically flaggable -> A: 0x01, B: 0x02, C: 0x04)
//Uses bitwise 'OR' operation in between the values and creates enumerated constants. For example, if 'Read':1, 'Write':2, then
ReadWrite= Read | Write = 1 | 2 = 3;
var myEnum = new Enum(['A', 'B', 'C']);

//define a flagged enum object to create a multicolor option; just pass an array
var myEnum = new Enum(['Black', 'Red', 'Green', 'Blue']);
...
```



# <a name="apidoc.module.enum.enum_2_4_0.prototype"></a>[module enum.enum_2_4_0.prototype](#apidoc.module.enum.enum_2_4_0.prototype)

#### <a name="apidoc.element.enum.enum_2_4_0.prototype.extend"></a>[function <span class="apidocSignatureSpan">enum.enum_2_4_0.prototype.</span>extend (map)](#apidoc.element.enum.enum_2_4_0.prototype.extend)
- description and source-code
```javascript
function extend(map) {
  if (map.length) {
    var array = map;
    map = {};

    for (var i = 0; i < array.length; i++) {
      var exponent = this._enumLastIndex + i;
      map[array[i]] = Math.pow(2, exponent);
    }

    for (var member in map) {
      guardReservedKeys(this._options.name, member);
      this[member] = new EnumItem(member, map[member], { ignoreCase: this._options.ignoreCase });
      this.enums.push(this[member]);
    }

    for (var key in this._enumMap) {
      map[key] = this._enumMap[key];
    }

    this._enumLastIndex += map.length;
    this._enumMap = map;

    if (this._options.freez) {
      this.freezeEnums(); //this will make instances of new Enum non-extensible
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.enum.enum_2_4_0.prototype.freezeEnums"></a>[function <span class="apidocSignatureSpan">enum.enum_2_4_0.prototype.</span>freezeEnums ()](#apidoc.element.enum.enum_2_4_0.prototype.freezeEnums)
- description and source-code
```javascript
function freezeEnums() {
  function envSupportsFreezing() {
    return Object.isFrozen && Object.isSealed && Object.getOwnPropertyNames && Object.getOwnPropertyDescriptor && Object.defineProperties
 && Object.__defineGetter__ && Object.__defineSetter__;
  }

  function freezer(o) {
    var props = Object.getOwnPropertyNames(o);
    props.forEach(function (p) {
      if (!Object.getOwnPropertyDescriptor(o, p).configurable) {
        return;
      }

      Object.defineProperties(o, p, { writable: false, configurable: false });
    });
    return o;
  }

  function getPropertyValue(value) {
    return value;
  }

  function deepFreezeEnums(o) {
    if (typeof o !== "object" || o === null || Object.isFrozen(o) || Object.isSealed(o)) {
      return;
    }
    for (var key in o) {
      if (o.hasOwnProperty(key)) {
        o.__defineGetter__(key, getPropertyValue.bind(null, o[key]));
        o.__defineSetter__(key, function throwPropertySetError(value) {
          throw TypeError("Cannot redefine property; Enum Type is not extensible.");
        });
        deepFreezeEnums(o[key]);
      }
    }
    if (Object.freeze) {
      Object.freeze(o);
    } else {
      freezer(o);
    }
  }

  if (envSupportsFreezing()) {
    deepFreezeEnums(this);
  }

  return this;
}
```
- example usage
```shell
...
      }
    }
    return true;
  };

  this.isFlaggable = isFlaggable();
  if (this._options.freez) {
    this.freezeEnums(); //this will make instances of Enum non-extensible
  }
}

/**
 * Returns the appropriate EnumItem key.
 * @param  {EnumItem || String || Number} key The object to get with.
 * @return {String}                           The get result.
...
```

#### <a name="apidoc.element.enum.enum_2_4_0.prototype.get"></a>[function <span class="apidocSignatureSpan">enum.enum_2_4_0.prototype.</span>get (key, offset)](#apidoc.element.enum.enum_2_4_0.prototype.get)
- description and source-code
```javascript
function get(key, offset) {
  if (key === null || key === undefined) {
    return;
  } // Buffer instance support, part of the ref Type interface
  if (isBuffer(key)) {
    key = key["readUInt32" + this._options.endianness](offset || 0);
  }

  if (EnumItem.isEnumItem(key)) {
    var foundIndex = indexOf.call(this.enums, key);
    if (foundIndex >= 0) {
      return key;
    }
    if (!this.isFlaggable || this.isFlaggable && key.key.indexOf(this._options.separator) < 0) {
      return;
    }
    return this.get(key.key);
  } else if (isString(key)) {

    var enums = this;
    if (this._options.ignoreCase) {
      enums = this.getLowerCaseEnums();
      key = key.toLowerCase();
    }

    if (key.indexOf(this._options.separator) > 0) {
      var parts = key.split(this._options.separator);

      var value = 0;
      for (var i = 0; i < parts.length; i++) {
        var part = parts[i];

        value |= enums[part].value;
      }

      return new EnumItem(key, value);
    } else {
      return enums[key];
    }
  } else {
    for (var m in this) {
      if (this.hasOwnProperty(m)) {
        if (this[m].value === key) {
          return this[m];
        }
      }
    }

    var result = null;

    if (this.isFlaggable) {
      for (var n in this) {
        if (this.hasOwnProperty(n)) {
          if ((key & this[n].value) !== 0) {
            if (result) {
              result += this._options.separator;
            } else {
              result = "";
            }
            result += n;
          }
        }
      }
    }

    return this.get(result || null);
  }
}
```
- example usage
```shell
...
var myEnum = new Enum(['A', 'B', 'C']);

//define a flagged enum object to create a multicolor option; just pass an array
var myEnum = new Enum(['Black', 'Red', 'Green', 'Blue']);
myEnum; //=> Enum {_options: Object, enums: Array[4], Black: EnumItem, Red: EnumItem, Green: EnumItem….....}
myEnum.isFlaggable; //=> true

for(var i=1; i<8; i++){ console.log(myEnum.get(i).value + '=> '+ myEnum.get(i).key)}
1=> Black
2=> Red
3=> Black | Red
4=> Green
5=> Black | Green
6=> Red | Green
7=> Black | Red | Green
...
```

#### <a name="apidoc.element.enum.enum_2_4_0.prototype.getKey"></a>[function <span class="apidocSignatureSpan">enum.enum_2_4_0.prototype.</span>getKey (value)](#apidoc.element.enum.enum_2_4_0.prototype.getKey)
- description and source-code
```javascript
function getKey(value) {
  var item = this.get(value);
  if (item) {
    return item.key;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.enum.enum_2_4_0.prototype.getValue"></a>[function <span class="apidocSignatureSpan">enum.enum_2_4_0.prototype.</span>getValue (key)](#apidoc.element.enum.enum_2_4_0.prototype.getValue)
- description and source-code
```javascript
function getValue(key) {
  var item = this.get(key);
  if (item) {
    return item.value;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.enum.enum_2_4_0.prototype.isDefined"></a>[function <span class="apidocSignatureSpan">enum.enum_2_4_0.prototype.</span>isDefined (enumItem)](#apidoc.element.enum.enum_2_4_0.prototype.isDefined)
- description and source-code
```javascript
function isDefined(enumItem) {
  var condition = function (e) {
    return e === enumItem;
  };
  if (isString(enumItem) || isNumber(enumItem)) {
    condition = function (e) {
      return e.is(enumItem);
    };
  }
  return this.enums.some(condition);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.enum.enum_2_4_0.prototype.set"></a>[function <span class="apidocSignatureSpan">enum.enum_2_4_0.prototype.</span>set (buffer, offset, value)](#apidoc.element.enum.enum_2_4_0.prototype.set)
- description and source-code
```javascript
function set(buffer, offset, value) {
  var item = this.get(value);
  if (item) {
    return buffer["writeUInt32" + this._options.endianness](item.value, offset || 0);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.enum.enum_2_4_0.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">enum.enum_2_4_0.prototype.</span>toJSON ()](#apidoc.element.enum.enum_2_4_0.prototype.toJSON)
- description and source-code
```javascript
function toJSON() {
  return this._enumMap;
}
```
- example usage
```shell
...
var myEnum = new Enum(['ONE', 'TWO', 'THREE'], { freez: true });

//define enum type without flag
var myEnum = new Enum({'None': 0, 'Black':1, 'Red': 2, 'Red2': 3, 'Green': 4, 'Blue': 5});
myEnum; //=>  Enum {_options: Object, enums: Array[6], None: EnumItem, Black: EnumItem, Red: EnumItem…........}
myEnum.isFlaggable; //=> false

myEnum.toJSON(); // returns {'None': 0, 'Black':1, 'Red': 2, 'Red2': 3, 'Green': 4, 'Blue': 5}
JSON.stringify(myEnum); // returns '{"None":0,"Black":1,"Red":2,"Red2":3,"Green":4,"Blue":5}'

for(var i=0; i<=5; i++){ console.log(myEnum.get(i).value + '=> '+ myEnum.get(i).key)}
0=> None
1=> Black
2=> Red
3=> Red2
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
