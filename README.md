# api documentation for  [mongoose-validator (v1.2.5)](https://github.com/leepowellcouk/mongoose-validator#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-mongoose-validator.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-mongoose-validator) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-mongoose-validator.svg)](https://travis-ci.org/npmdoc/node-npmdoc-mongoose-validator)
#### Validators for mongoose models utilising validator.js

[![NPM](https://nodei.co/npm/mongoose-validator.png?downloads=true)](https://www.npmjs.com/package/mongoose-validator)

[![apidoc](https://npmdoc.github.io/node-npmdoc-mongoose-validator/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-mongoose-validator_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-mongoose-validator/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-mongoose-validator/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-mongoose-validator/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Lee Powell",
        "email": "lee@leepowell.co.uk",
        "url": "https://leepowell.co.uk"
    },
    "bugs": {
        "url": "https://github.com/leepowellcouk/mongoose-validator/issues"
    },
    "contributors": [
        {
            "name": "Francesco Pasqua",
            "url": "https://github.com/cesconix/"
        },
        {
            "name": "Igor Escobar",
            "url": "https://github.com/igorescobar/"
        },
        {
            "name": "Todd Bluhm",
            "url": "https://github.com/toddbluhm/"
        },
        {
            "name": "Subash Pathak",
            "url": "https://github.com/subash/"
        },
        {
            "name": "Kristijan Sedlak",
            "url": "https://github.com/xpepermint"
        },
        {
            "name": "Eric Saboia",
            "url": "https://github.com/ericsaboia"
        },
        {
            "name": "Rob Rodriguez",
            "url": "https://github.com/rodriguise"
        }
    ],
    "dependencies": {
        "underscore": "^1.8.3",
        "validator": "^4.0.2"
    },
    "description": "Validators for mongoose models utilising validator.js",
    "devDependencies": {
        "mocha": "^2.2.5",
        "mongoose": "^4.0.5",
        "should": "^6.0.3"
    },
    "directories": {},
    "dist": {
        "shasum": "20ecce963d2e7ea9c244a35494aa73c435a958db",
        "tarball": "https://registry.npmjs.org/mongoose-validator/-/mongoose-validator-1.2.5.tgz"
    },
    "engines": {
        "node": "*"
    },
    "gitHead": "571f3f90f9d353b17ec9731cceba80a86681c069",
    "homepage": "https://github.com/leepowellcouk/mongoose-validator#readme",
    "keywords": [
        "mongoose",
        "validate",
        "validation",
        "models",
        "schema"
    ],
    "license": "MIT",
    "main": "./lib/mongoose-validator",
    "maintainers": [
        {
            "name": "leepowellcouk",
            "email": "lee@leepowell.co.uk"
        }
    ],
    "name": "mongoose-validator",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/leepowellcouk/mongoose-validator.git"
    },
    "scripts": {
        "test": "mocha -R list"
    },
    "version": "1.2.5"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module mongoose-validator](#apidoc.module.mongoose-validator)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.</span>extend (name, fn, errorMsg)](#apidoc.element.mongoose-validator.extend)
1.  object <span class="apidocSignatureSpan">mongoose-validator.</span>defaultErrorMessages
1.  object <span class="apidocSignatureSpan">mongoose-validator.</span>validatorjs

#### [module mongoose-validator.validatorjs](#apidoc.module.mongoose-validator.validatorjs)
1.  boolean <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>coerce
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>blacklist ()](#apidoc.element.mongoose-validator.validatorjs.blacklist)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>contains ()](#apidoc.element.mongoose-validator.validatorjs.contains)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>deprecation ()](#apidoc.element.mongoose-validator.validatorjs.deprecation)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>equals ()](#apidoc.element.mongoose-validator.validatorjs.equals)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>escape ()](#apidoc.element.mongoose-validator.validatorjs.escape)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>extend (name, fn)](#apidoc.element.mongoose-validator.validatorjs.extend)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>init ()](#apidoc.element.mongoose-validator.validatorjs.init)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isAfter ()](#apidoc.element.mongoose-validator.validatorjs.isAfter)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isAlpha ()](#apidoc.element.mongoose-validator.validatorjs.isAlpha)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isAlphanumeric ()](#apidoc.element.mongoose-validator.validatorjs.isAlphanumeric)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isAscii ()](#apidoc.element.mongoose-validator.validatorjs.isAscii)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isBase64 ()](#apidoc.element.mongoose-validator.validatorjs.isBase64)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isBefore ()](#apidoc.element.mongoose-validator.validatorjs.isBefore)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isBoolean ()](#apidoc.element.mongoose-validator.validatorjs.isBoolean)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isByteLength ()](#apidoc.element.mongoose-validator.validatorjs.isByteLength)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isCreditCard ()](#apidoc.element.mongoose-validator.validatorjs.isCreditCard)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isCurrency ()](#apidoc.element.mongoose-validator.validatorjs.isCurrency)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isDate ()](#apidoc.element.mongoose-validator.validatorjs.isDate)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isDecimal ()](#apidoc.element.mongoose-validator.validatorjs.isDecimal)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isDivisibleBy ()](#apidoc.element.mongoose-validator.validatorjs.isDivisibleBy)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isEmail ()](#apidoc.element.mongoose-validator.validatorjs.isEmail)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isFQDN ()](#apidoc.element.mongoose-validator.validatorjs.isFQDN)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isFloat ()](#apidoc.element.mongoose-validator.validatorjs.isFloat)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isFullWidth ()](#apidoc.element.mongoose-validator.validatorjs.isFullWidth)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isHalfWidth ()](#apidoc.element.mongoose-validator.validatorjs.isHalfWidth)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isHexColor ()](#apidoc.element.mongoose-validator.validatorjs.isHexColor)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isHexadecimal ()](#apidoc.element.mongoose-validator.validatorjs.isHexadecimal)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isIP ()](#apidoc.element.mongoose-validator.validatorjs.isIP)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isISBN ()](#apidoc.element.mongoose-validator.validatorjs.isISBN)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isISIN ()](#apidoc.element.mongoose-validator.validatorjs.isISIN)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isISO8601 ()](#apidoc.element.mongoose-validator.validatorjs.isISO8601)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isIn ()](#apidoc.element.mongoose-validator.validatorjs.isIn)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isInt ()](#apidoc.element.mongoose-validator.validatorjs.isInt)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isJSON ()](#apidoc.element.mongoose-validator.validatorjs.isJSON)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isLength ()](#apidoc.element.mongoose-validator.validatorjs.isLength)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isLowercase ()](#apidoc.element.mongoose-validator.validatorjs.isLowercase)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isMACAddress ()](#apidoc.element.mongoose-validator.validatorjs.isMACAddress)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isMobilePhone ()](#apidoc.element.mongoose-validator.validatorjs.isMobilePhone)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isMongoId ()](#apidoc.element.mongoose-validator.validatorjs.isMongoId)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isMultibyte ()](#apidoc.element.mongoose-validator.validatorjs.isMultibyte)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isNull ()](#apidoc.element.mongoose-validator.validatorjs.isNull)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isNumeric ()](#apidoc.element.mongoose-validator.validatorjs.isNumeric)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isServerSide ()](#apidoc.element.mongoose-validator.validatorjs.isServerSide)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isSurrogatePair ()](#apidoc.element.mongoose-validator.validatorjs.isSurrogatePair)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isURL ()](#apidoc.element.mongoose-validator.validatorjs.isURL)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isUUID ()](#apidoc.element.mongoose-validator.validatorjs.isUUID)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isUppercase ()](#apidoc.element.mongoose-validator.validatorjs.isUppercase)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isVariableWidth ()](#apidoc.element.mongoose-validator.validatorjs.isVariableWidth)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isWhitelisted ()](#apidoc.element.mongoose-validator.validatorjs.isWhitelisted)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>ltrim ()](#apidoc.element.mongoose-validator.validatorjs.ltrim)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>matches ()](#apidoc.element.mongoose-validator.validatorjs.matches)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>normalizeEmail ()](#apidoc.element.mongoose-validator.validatorjs.normalizeEmail)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>rtrim ()](#apidoc.element.mongoose-validator.validatorjs.rtrim)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>stripLow ()](#apidoc.element.mongoose-validator.validatorjs.stripLow)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>toBoolean ()](#apidoc.element.mongoose-validator.validatorjs.toBoolean)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>toDate (date)](#apidoc.element.mongoose-validator.validatorjs.toDate)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>toFloat ()](#apidoc.element.mongoose-validator.validatorjs.toFloat)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>toInt ()](#apidoc.element.mongoose-validator.validatorjs.toInt)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>toString (input)](#apidoc.element.mongoose-validator.validatorjs.toString)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>trim ()](#apidoc.element.mongoose-validator.validatorjs.trim)
1.  [function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>whitelist ()](#apidoc.element.mongoose-validator.validatorjs.whitelist)
1.  string <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>version



# <a name="apidoc.module.mongoose-validator"></a>[module mongoose-validator](#apidoc.module.mongoose-validator)

#### <a name="apidoc.element.mongoose-validator.extend"></a>[function <span class="apidocSignatureSpan">mongoose-validator.</span>extend (name, fn, errorMsg)](#apidoc.element.mongoose-validator.extend)
- description and source-code
```javascript
extend = function (name, fn, errorMsg) {
  if (!validatorjs[name]) {
    validatorjs[name]   = function () { return fn.apply(this, Array.prototype.slice.call(arguments)); };
    errorMessages[name] = errorMsg || 'Error';
  }
  else {
    throw new Error('Validator '' +  name + '' already exists on validator.js');
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.mongoose-validator.validatorjs"></a>[module mongoose-validator.validatorjs](#apidoc.module.mongoose-validator.validatorjs)

#### <a name="apidoc.element.mongoose-validator.validatorjs.blacklist"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>blacklist ()](#apidoc.element.mongoose-validator.validatorjs.blacklist)
- description and source-code
```javascript
blacklist = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.contains"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>contains ()](#apidoc.element.mongoose-validator.validatorjs.contains)
- description and source-code
```javascript
contains = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.deprecation"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>deprecation ()](#apidoc.element.mongoose-validator.validatorjs.deprecation)
- description and source-code
```javascript
deprecation = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.equals"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>equals ()](#apidoc.element.mongoose-validator.validatorjs.equals)
- description and source-code
```javascript
equals = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.escape"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>escape ()](#apidoc.element.mongoose-validator.validatorjs.escape)
- description and source-code
```javascript
escape = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.extend"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>extend (name, fn)](#apidoc.element.mongoose-validator.validatorjs.extend)
- description and source-code
```javascript
extend = function (name, fn) {
    validator[name] = function () {
        var args = Array.prototype.slice.call(arguments);
        args[0] = validator.toString(args[0]);
        return fn.apply(validator, args);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.init"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>init ()](#apidoc.element.mongoose-validator.validatorjs.init)
- description and source-code
```javascript
init = function () {
    for (var name in validator) {
        if (typeof validator[name] !== 'function' || name === 'toString' ||
                name === 'toDate' || name === 'extend' || name === 'init' ||
                name === 'isServerSide') {
            continue;
        }
        validator.extend(name, validator[name]);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isAfter"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isAfter ()](#apidoc.element.mongoose-validator.validatorjs.isAfter)
- description and source-code
```javascript
isAfter = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isAlpha"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isAlpha ()](#apidoc.element.mongoose-validator.validatorjs.isAlpha)
- description and source-code
```javascript
isAlpha = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isAlphanumeric"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isAlphanumeric ()](#apidoc.element.mongoose-validator.validatorjs.isAlphanumeric)
- description and source-code
```javascript
isAlphanumeric = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isAscii"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isAscii ()](#apidoc.element.mongoose-validator.validatorjs.isAscii)
- description and source-code
```javascript
isAscii = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isBase64"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isBase64 ()](#apidoc.element.mongoose-validator.validatorjs.isBase64)
- description and source-code
```javascript
isBase64 = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isBefore"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isBefore ()](#apidoc.element.mongoose-validator.validatorjs.isBefore)
- description and source-code
```javascript
isBefore = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isBoolean"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isBoolean ()](#apidoc.element.mongoose-validator.validatorjs.isBoolean)
- description and source-code
```javascript
isBoolean = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isByteLength"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isByteLength ()](#apidoc.element.mongoose-validator.validatorjs.isByteLength)
- description and source-code
```javascript
isByteLength = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isCreditCard"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isCreditCard ()](#apidoc.element.mongoose-validator.validatorjs.isCreditCard)
- description and source-code
```javascript
isCreditCard = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isCurrency"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isCurrency ()](#apidoc.element.mongoose-validator.validatorjs.isCurrency)
- description and source-code
```javascript
isCurrency = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isDate"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isDate ()](#apidoc.element.mongoose-validator.validatorjs.isDate)
- description and source-code
```javascript
isDate = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isDecimal"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isDecimal ()](#apidoc.element.mongoose-validator.validatorjs.isDecimal)
- description and source-code
```javascript
isDecimal = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isDivisibleBy"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isDivisibleBy ()](#apidoc.element.mongoose-validator.validatorjs.isDivisibleBy)
- description and source-code
```javascript
isDivisibleBy = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isEmail"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isEmail ()](#apidoc.element.mongoose-validator.validatorjs.isEmail)
- description and source-code
```javascript
isEmail = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isFQDN"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isFQDN ()](#apidoc.element.mongoose-validator.validatorjs.isFQDN)
- description and source-code
```javascript
isFQDN = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isFloat"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isFloat ()](#apidoc.element.mongoose-validator.validatorjs.isFloat)
- description and source-code
```javascript
isFloat = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isFullWidth"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isFullWidth ()](#apidoc.element.mongoose-validator.validatorjs.isFullWidth)
- description and source-code
```javascript
isFullWidth = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isHalfWidth"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isHalfWidth ()](#apidoc.element.mongoose-validator.validatorjs.isHalfWidth)
- description and source-code
```javascript
isHalfWidth = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isHexColor"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isHexColor ()](#apidoc.element.mongoose-validator.validatorjs.isHexColor)
- description and source-code
```javascript
isHexColor = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isHexadecimal"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isHexadecimal ()](#apidoc.element.mongoose-validator.validatorjs.isHexadecimal)
- description and source-code
```javascript
isHexadecimal = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isIP"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isIP ()](#apidoc.element.mongoose-validator.validatorjs.isIP)
- description and source-code
```javascript
isIP = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isISBN"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isISBN ()](#apidoc.element.mongoose-validator.validatorjs.isISBN)
- description and source-code
```javascript
isISBN = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isISIN"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isISIN ()](#apidoc.element.mongoose-validator.validatorjs.isISIN)
- description and source-code
```javascript
isISIN = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isISO8601"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isISO8601 ()](#apidoc.element.mongoose-validator.validatorjs.isISO8601)
- description and source-code
```javascript
isISO8601 = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isIn"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isIn ()](#apidoc.element.mongoose-validator.validatorjs.isIn)
- description and source-code
```javascript
isIn = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isInt"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isInt ()](#apidoc.element.mongoose-validator.validatorjs.isInt)
- description and source-code
```javascript
isInt = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isJSON"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isJSON ()](#apidoc.element.mongoose-validator.validatorjs.isJSON)
- description and source-code
```javascript
isJSON = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isLength"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isLength ()](#apidoc.element.mongoose-validator.validatorjs.isLength)
- description and source-code
```javascript
isLength = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isLowercase"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isLowercase ()](#apidoc.element.mongoose-validator.validatorjs.isLowercase)
- description and source-code
```javascript
isLowercase = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isMACAddress"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isMACAddress ()](#apidoc.element.mongoose-validator.validatorjs.isMACAddress)
- description and source-code
```javascript
isMACAddress = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isMobilePhone"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isMobilePhone ()](#apidoc.element.mongoose-validator.validatorjs.isMobilePhone)
- description and source-code
```javascript
isMobilePhone = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isMongoId"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isMongoId ()](#apidoc.element.mongoose-validator.validatorjs.isMongoId)
- description and source-code
```javascript
isMongoId = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isMultibyte"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isMultibyte ()](#apidoc.element.mongoose-validator.validatorjs.isMultibyte)
- description and source-code
```javascript
isMultibyte = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isNull"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isNull ()](#apidoc.element.mongoose-validator.validatorjs.isNull)
- description and source-code
```javascript
isNull = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isNumeric"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isNumeric ()](#apidoc.element.mongoose-validator.validatorjs.isNumeric)
- description and source-code
```javascript
isNumeric = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isServerSide"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isServerSide ()](#apidoc.element.mongoose-validator.validatorjs.isServerSide)
- description and source-code
```javascript
isServerSide = function () {
    return typeof module === 'object' && module &&
        typeof module.exports === 'object' &&
        typeof process === 'object' &&
        typeof require === 'function';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isSurrogatePair"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isSurrogatePair ()](#apidoc.element.mongoose-validator.validatorjs.isSurrogatePair)
- description and source-code
```javascript
isSurrogatePair = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isURL"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isURL ()](#apidoc.element.mongoose-validator.validatorjs.isURL)
- description and source-code
```javascript
isURL = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isUUID"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isUUID ()](#apidoc.element.mongoose-validator.validatorjs.isUUID)
- description and source-code
```javascript
isUUID = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isUppercase"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isUppercase ()](#apidoc.element.mongoose-validator.validatorjs.isUppercase)
- description and source-code
```javascript
isUppercase = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isVariableWidth"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isVariableWidth ()](#apidoc.element.mongoose-validator.validatorjs.isVariableWidth)
- description and source-code
```javascript
isVariableWidth = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.isWhitelisted"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>isWhitelisted ()](#apidoc.element.mongoose-validator.validatorjs.isWhitelisted)
- description and source-code
```javascript
isWhitelisted = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.ltrim"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>ltrim ()](#apidoc.element.mongoose-validator.validatorjs.ltrim)
- description and source-code
```javascript
ltrim = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.matches"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>matches ()](#apidoc.element.mongoose-validator.validatorjs.matches)
- description and source-code
```javascript
matches = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.normalizeEmail"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>normalizeEmail ()](#apidoc.element.mongoose-validator.validatorjs.normalizeEmail)
- description and source-code
```javascript
normalizeEmail = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.rtrim"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>rtrim ()](#apidoc.element.mongoose-validator.validatorjs.rtrim)
- description and source-code
```javascript
rtrim = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.stripLow"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>stripLow ()](#apidoc.element.mongoose-validator.validatorjs.stripLow)
- description and source-code
```javascript
stripLow = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.toBoolean"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>toBoolean ()](#apidoc.element.mongoose-validator.validatorjs.toBoolean)
- description and source-code
```javascript
toBoolean = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.toDate"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>toDate (date)](#apidoc.element.mongoose-validator.validatorjs.toDate)
- description and source-code
```javascript
toDate = function (date) {
    if (Object.prototype.toString.call(date) === '[object Date]') {
        return date;
    }
    date = Date.parse(date);
    return !isNaN(date) ? new Date(date) : null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.toFloat"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>toFloat ()](#apidoc.element.mongoose-validator.validatorjs.toFloat)
- description and source-code
```javascript
toFloat = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.toInt"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>toInt ()](#apidoc.element.mongoose-validator.validatorjs.toInt)
- description and source-code
```javascript
toInt = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.toString"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>toString (input)](#apidoc.element.mongoose-validator.validatorjs.toString)
- description and source-code
```javascript
toString = function (input) {
    if (typeof input !== 'string') {
        // The library validates strings only. Currently it coerces all input to a string, but this
        // will go away in an upcoming major version change. Print a deprecation notice for now
        if (!validator.coerce) {
            throw new Error('this library validates strings only');
        }
        validator.deprecation('you tried to validate a ' + typeof input + ' but this library ' +
                '(validator.js) validates strings only. Please update your code as this will ' +
                'be an error soon.');
    }
    if (typeof input === 'object' && input !== null) {
        if (typeof input.toString === 'function') {
            input = input.toString();
        } else {
            input = '[object Object]';
        }
    } else if (input === null || typeof input === 'undefined' || (isNaN(input) && !input.length)) {
        input = '';
    }
    return '' + input;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.trim"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>trim ()](#apidoc.element.mongoose-validator.validatorjs.trim)
- description and source-code
```javascript
trim = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.mongoose-validator.validatorjs.whitelist"></a>[function <span class="apidocSignatureSpan">mongoose-validator.validatorjs.</span>whitelist ()](#apidoc.element.mongoose-validator.validatorjs.whitelist)
- description and source-code
```javascript
whitelist = function () {
    var args = Array.prototype.slice.call(arguments);
    args[0] = validator.toString(args[0]);
    return fn.apply(validator, args);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
