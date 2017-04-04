# api documentation for  [html-entities (v1.2.0)](https://github.com/mdevils/node-html-entities#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-html-entities.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-html-entities) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-html-entities.svg)](https://travis-ci.org/npmdoc/node-npmdoc-html-entities)
#### Faster HTML entities encode/decode library.

[![NPM](https://nodei.co/npm/html-entities.png?downloads=true)](https://www.npmjs.com/package/html-entities)

[![apidoc](https://npmdoc.github.io/node-npmdoc-html-entities/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-html-entities_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-html-entities/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-html-entities/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-html-entities/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Marat Dulin",
        "email": "mdevils@yandex.ru"
    },
    "bugs": {
        "url": "https://github.com/mdevils/node-html-entities/issues"
    },
    "dependencies": {},
    "description": "Faster HTML entities encode/decode library.",
    "devDependencies": {
        "chai": "^1.9.1",
        "coveralls": "^2.11.2",
        "entities": "*",
        "mocha": "^1.21.4",
        "node-html-encoder": "*",
        "unit-coverage": "^3.0.1"
    },
    "directories": {},
    "dist": {
        "shasum": "41948caf85ce82fed36e4e6a0ed371a6664379e2",
        "tarball": "https://registry.npmjs.org/html-entities/-/html-entities-1.2.0.tgz"
    },
    "engines": [
        "node >= 0.4.0"
    ],
    "files": [
        "index.js",
        "lib",
        "LICENSE"
    ],
    "gitHead": "3a2cd397697c872325f526bb422bdee74f089cda",
    "homepage": "https://github.com/mdevils/node-html-entities#readme",
    "keywords": [
        "html",
        "html entities",
        "html entities encode",
        "html entities decode",
        "entities",
        "entities encode",
        "entities decode"
    ],
    "license": "MIT",
    "main": "index",
    "maintainers": [
        {
            "name": "mdevils",
            "email": "mdevils@yandex.ru"
        }
    ],
    "name": "html-entities",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mdevils/node-html-entities.git"
    },
    "scripts": {
        "benchmark": "node benchmark/benchmark",
        "coverage": "unit-coverage run -p common",
        "coverage-html": "unit-coverage run -p common -r html -o coverage.html",
        "test": "mocha --recursive -R spec test",
        "travis": "npm test && unit-coverage run -p common -r lcov -o coverage.lcov && cat coverage.lcov | coveralls"
    },
    "unit-coverage": {
        "common": [
            "-s",
            "lib/**/*.js",
            "-t",
            "test/**/*.js"
        ]
    },
    "version": "1.2.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module html-entities](#apidoc.module.html-entities)
1.  [function <span class="apidocSignatureSpan">html-entities.</span>AllHtmlEntities ()](#apidoc.element.html-entities.AllHtmlEntities)
1.  [function <span class="apidocSignatureSpan">html-entities.</span>Html4Entities ()](#apidoc.element.html-entities.Html4Entities)
1.  [function <span class="apidocSignatureSpan">html-entities.</span>Html5Entities ()](#apidoc.element.html-entities.Html5Entities)
1.  [function <span class="apidocSignatureSpan">html-entities.</span>XmlEntities ()](#apidoc.element.html-entities.XmlEntities)
1.  object <span class="apidocSignatureSpan">html-entities.</span>Html4Entities.prototype
1.  object <span class="apidocSignatureSpan">html-entities.</span>Html5Entities.prototype
1.  object <span class="apidocSignatureSpan">html-entities.</span>XmlEntities.prototype

#### [module html-entities.Html4Entities](#apidoc.module.html-entities.Html4Entities)
1.  [function <span class="apidocSignatureSpan">html-entities.</span>Html4Entities ()](#apidoc.element.html-entities.Html4Entities.Html4Entities)
1.  [function <span class="apidocSignatureSpan">html-entities.Html4Entities.</span>decode (str)](#apidoc.element.html-entities.Html4Entities.decode)
1.  [function <span class="apidocSignatureSpan">html-entities.Html4Entities.</span>encode (str)](#apidoc.element.html-entities.Html4Entities.encode)
1.  [function <span class="apidocSignatureSpan">html-entities.Html4Entities.</span>encodeNonASCII (str)](#apidoc.element.html-entities.Html4Entities.encodeNonASCII)
1.  [function <span class="apidocSignatureSpan">html-entities.Html4Entities.</span>encodeNonUTF (str)](#apidoc.element.html-entities.Html4Entities.encodeNonUTF)

#### [module html-entities.Html4Entities.prototype](#apidoc.module.html-entities.Html4Entities.prototype)
1.  [function <span class="apidocSignatureSpan">html-entities.Html4Entities.prototype.</span>decode (str)](#apidoc.element.html-entities.Html4Entities.prototype.decode)
1.  [function <span class="apidocSignatureSpan">html-entities.Html4Entities.prototype.</span>encode (str)](#apidoc.element.html-entities.Html4Entities.prototype.encode)
1.  [function <span class="apidocSignatureSpan">html-entities.Html4Entities.prototype.</span>encodeNonASCII (str)](#apidoc.element.html-entities.Html4Entities.prototype.encodeNonASCII)
1.  [function <span class="apidocSignatureSpan">html-entities.Html4Entities.prototype.</span>encodeNonUTF (str)](#apidoc.element.html-entities.Html4Entities.prototype.encodeNonUTF)

#### [module html-entities.Html5Entities](#apidoc.module.html-entities.Html5Entities)
1.  [function <span class="apidocSignatureSpan">html-entities.</span>Html5Entities ()](#apidoc.element.html-entities.Html5Entities.Html5Entities)
1.  [function <span class="apidocSignatureSpan">html-entities.Html5Entities.</span>decode (str)](#apidoc.element.html-entities.Html5Entities.decode)
1.  [function <span class="apidocSignatureSpan">html-entities.Html5Entities.</span>encode (str)](#apidoc.element.html-entities.Html5Entities.encode)
1.  [function <span class="apidocSignatureSpan">html-entities.Html5Entities.</span>encodeNonASCII (str)](#apidoc.element.html-entities.Html5Entities.encodeNonASCII)
1.  [function <span class="apidocSignatureSpan">html-entities.Html5Entities.</span>encodeNonUTF (str)](#apidoc.element.html-entities.Html5Entities.encodeNonUTF)

#### [module html-entities.Html5Entities.prototype](#apidoc.module.html-entities.Html5Entities.prototype)
1.  [function <span class="apidocSignatureSpan">html-entities.Html5Entities.prototype.</span>decode (str)](#apidoc.element.html-entities.Html5Entities.prototype.decode)
1.  [function <span class="apidocSignatureSpan">html-entities.Html5Entities.prototype.</span>encode (str)](#apidoc.element.html-entities.Html5Entities.prototype.encode)
1.  [function <span class="apidocSignatureSpan">html-entities.Html5Entities.prototype.</span>encodeNonASCII (str)](#apidoc.element.html-entities.Html5Entities.prototype.encodeNonASCII)
1.  [function <span class="apidocSignatureSpan">html-entities.Html5Entities.prototype.</span>encodeNonUTF (str)](#apidoc.element.html-entities.Html5Entities.prototype.encodeNonUTF)

#### [module html-entities.XmlEntities](#apidoc.module.html-entities.XmlEntities)
1.  [function <span class="apidocSignatureSpan">html-entities.</span>XmlEntities ()](#apidoc.element.html-entities.XmlEntities.XmlEntities)
1.  [function <span class="apidocSignatureSpan">html-entities.XmlEntities.</span>decode (str)](#apidoc.element.html-entities.XmlEntities.decode)
1.  [function <span class="apidocSignatureSpan">html-entities.XmlEntities.</span>encode (str)](#apidoc.element.html-entities.XmlEntities.encode)
1.  [function <span class="apidocSignatureSpan">html-entities.XmlEntities.</span>encodeNonASCII (str)](#apidoc.element.html-entities.XmlEntities.encodeNonASCII)
1.  [function <span class="apidocSignatureSpan">html-entities.XmlEntities.</span>encodeNonUTF (str)](#apidoc.element.html-entities.XmlEntities.encodeNonUTF)

#### [module html-entities.XmlEntities.prototype](#apidoc.module.html-entities.XmlEntities.prototype)
1.  [function <span class="apidocSignatureSpan">html-entities.XmlEntities.prototype.</span>decode (str)](#apidoc.element.html-entities.XmlEntities.prototype.decode)
1.  [function <span class="apidocSignatureSpan">html-entities.XmlEntities.prototype.</span>encode (str)](#apidoc.element.html-entities.XmlEntities.prototype.encode)
1.  [function <span class="apidocSignatureSpan">html-entities.XmlEntities.prototype.</span>encodeNonASCII (str)](#apidoc.element.html-entities.XmlEntities.prototype.encodeNonASCII)
1.  [function <span class="apidocSignatureSpan">html-entities.XmlEntities.prototype.</span>encodeNonUTF (str)](#apidoc.element.html-entities.XmlEntities.prototype.encodeNonUTF)



# <a name="apidoc.module.html-entities"></a>[module html-entities](#apidoc.module.html-entities)

#### <a name="apidoc.element.html-entities.AllHtmlEntities"></a>[function <span class="apidocSignatureSpan">html-entities.</span>AllHtmlEntities ()](#apidoc.element.html-entities.AllHtmlEntities)
- description and source-code
```javascript
function Html5Entities() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html-entities.Html4Entities"></a>[function <span class="apidocSignatureSpan">html-entities.</span>Html4Entities ()](#apidoc.element.html-entities.Html4Entities)
- description and source-code
```javascript
function Html4Entities() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html-entities.Html5Entities"></a>[function <span class="apidocSignatureSpan">html-entities.</span>Html5Entities ()](#apidoc.element.html-entities.Html5Entities)
- description and source-code
```javascript
function Html5Entities() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html-entities.XmlEntities"></a>[function <span class="apidocSignatureSpan">html-entities.</span>XmlEntities ()](#apidoc.element.html-entities.XmlEntities)
- description and source-code
```javascript
function XmlEntities() {}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.html-entities.Html4Entities"></a>[module html-entities.Html4Entities](#apidoc.module.html-entities.Html4Entities)

#### <a name="apidoc.element.html-entities.Html4Entities.Html4Entities"></a>[function <span class="apidocSignatureSpan">html-entities.</span>Html4Entities ()](#apidoc.element.html-entities.Html4Entities.Html4Entities)
- description and source-code
```javascript
function Html4Entities() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html-entities.Html4Entities.decode"></a>[function <span class="apidocSignatureSpan">html-entities.Html4Entities.</span>decode (str)](#apidoc.element.html-entities.Html4Entities.decode)
- description and source-code
```javascript
decode = function (str) {
    return new Html4Entities().decode(str);
}
```
- example usage
```shell
...
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####


'''javascript
var Entities = require('html-entities').AllHtmlEntities;
...
```

#### <a name="apidoc.element.html-entities.Html4Entities.encode"></a>[function <span class="apidocSignatureSpan">html-entities.Html4Entities.</span>encode (str)](#apidoc.element.html-entities.Html4Entities.encode)
- description and source-code
```javascript
encode = function (str) {
    return new Html4Entities().encode(str);
}
```
- example usage
```shell
...
HTML validity and XSS attack prevention you can achieve from XmlEntities class.

'''javascript
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####
...
```

#### <a name="apidoc.element.html-entities.Html4Entities.encodeNonASCII"></a>[function <span class="apidocSignatureSpan">html-entities.Html4Entities.</span>encodeNonASCII (str)](#apidoc.element.html-entities.Html4Entities.encodeNonASCII)
- description and source-code
```javascript
encodeNonASCII = function (str) {
    return new Html4Entities().encodeNonASCII(str);
}
```
- example usage
```shell
...
'''javascript
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####


'''javascript
...
```

#### <a name="apidoc.element.html-entities.Html4Entities.encodeNonUTF"></a>[function <span class="apidocSignatureSpan">html-entities.Html4Entities.</span>encodeNonUTF (str)](#apidoc.element.html-entities.Html4Entities.encodeNonUTF)
- description and source-code
```javascript
encodeNonUTF = function (str) {
    return new Html4Entities().encodeNonUTF(str);
}
```
- example usage
```shell
...

'''javascript
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####
...
```



# <a name="apidoc.module.html-entities.Html4Entities.prototype"></a>[module html-entities.Html4Entities.prototype](#apidoc.module.html-entities.Html4Entities.prototype)

#### <a name="apidoc.element.html-entities.Html4Entities.prototype.decode"></a>[function <span class="apidocSignatureSpan">html-entities.Html4Entities.prototype.</span>decode (str)](#apidoc.element.html-entities.Html4Entities.prototype.decode)
- description and source-code
```javascript
decode = function (str) {
    if (str.length === 0) {
        return '';
    }
    return str.replace(/&(#?[\w\d]+);?/g, function(s, entity) {
        var chr;
        if (entity.charAt(0) === "#") {
            var code = entity.charAt(1).toLowerCase() === 'x' ?
                parseInt(entity.substr(2), 16) :
                parseInt(entity.substr(1));

            if (!(isNaN(code) || code < -32768 || code > 65535)) {
                chr = String.fromCharCode(code);
            }
        } else {
            chr = alphaIndex[entity];
        }
        return chr || s;
    });
}
```
- example usage
```shell
...
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####


'''javascript
var Entities = require('html-entities').AllHtmlEntities;
...
```

#### <a name="apidoc.element.html-entities.Html4Entities.prototype.encode"></a>[function <span class="apidocSignatureSpan">html-entities.Html4Entities.prototype.</span>encode (str)](#apidoc.element.html-entities.Html4Entities.prototype.encode)
- description and source-code
```javascript
encode = function (str) {
    var strLength = str.length;
    if (strLength === 0) {
        return '';
    }
    var result = '';
    var i = 0;
    while (i < strLength) {
        var alpha = numIndex[str.charCodeAt(i)];
        result += alpha ? "&" + alpha + ";" : str.charAt(i);
        i++;
    }
    return result;
}
```
- example usage
```shell
...
HTML validity and XSS attack prevention you can achieve from XmlEntities class.

'''javascript
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####
...
```

#### <a name="apidoc.element.html-entities.Html4Entities.prototype.encodeNonASCII"></a>[function <span class="apidocSignatureSpan">html-entities.Html4Entities.prototype.</span>encodeNonASCII (str)](#apidoc.element.html-entities.Html4Entities.prototype.encodeNonASCII)
- description and source-code
```javascript
encodeNonASCII = function (str) {
    var strLength = str.length;
    if (strLength === 0) {
        return '';
    }
    var result = '';
    var i = 0;
    while (i < strLength) {
        var c = str.charCodeAt(i);
        if (c <= 255) {
            result += str[i++];
            continue;
        }
        result += '&#' + c + ';';
        i++;
    }
    return result;
}
```
- example usage
```shell
...
'''javascript
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####


'''javascript
...
```

#### <a name="apidoc.element.html-entities.Html4Entities.prototype.encodeNonUTF"></a>[function <span class="apidocSignatureSpan">html-entities.Html4Entities.prototype.</span>encodeNonUTF (str)](#apidoc.element.html-entities.Html4Entities.prototype.encodeNonUTF)
- description and source-code
```javascript
encodeNonUTF = function (str) {
    var strLength = str.length;
    if (strLength === 0) {
        return '';
    }
    var result = '';
    var i = 0;
    while (i < strLength) {
        var cc = str.charCodeAt(i);
        var alpha = numIndex[cc];
        if (alpha) {
            result += "&" + alpha + ";";
        } else if (cc < 32 || cc > 126) {
            result += "&#" + cc + ";";
        } else {
            result += str.charAt(i);
        }
        i++;
    }
    return result;
}
```
- example usage
```shell
...

'''javascript
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####
...
```



# <a name="apidoc.module.html-entities.Html5Entities"></a>[module html-entities.Html5Entities](#apidoc.module.html-entities.Html5Entities)

#### <a name="apidoc.element.html-entities.Html5Entities.Html5Entities"></a>[function <span class="apidocSignatureSpan">html-entities.</span>Html5Entities ()](#apidoc.element.html-entities.Html5Entities.Html5Entities)
- description and source-code
```javascript
function Html5Entities() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html-entities.Html5Entities.decode"></a>[function <span class="apidocSignatureSpan">html-entities.Html5Entities.</span>decode (str)](#apidoc.element.html-entities.Html5Entities.decode)
- description and source-code
```javascript
decode = function (str) {
   return new Html5Entities().decode(str);
}
```
- example usage
```shell
...
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####


'''javascript
var Entities = require('html-entities').AllHtmlEntities;
...
```

#### <a name="apidoc.element.html-entities.Html5Entities.encode"></a>[function <span class="apidocSignatureSpan">html-entities.Html5Entities.</span>encode (str)](#apidoc.element.html-entities.Html5Entities.encode)
- description and source-code
```javascript
encode = function (str) {
   return new Html5Entities().encode(str);
}
```
- example usage
```shell
...
HTML validity and XSS attack prevention you can achieve from XmlEntities class.

'''javascript
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####
...
```

#### <a name="apidoc.element.html-entities.Html5Entities.encodeNonASCII"></a>[function <span class="apidocSignatureSpan">html-entities.Html5Entities.</span>encodeNonASCII (str)](#apidoc.element.html-entities.Html5Entities.encodeNonASCII)
- description and source-code
```javascript
encodeNonASCII = function (str) {
   return new Html5Entities().encodeNonASCII(str);
}
```
- example usage
```shell
...
'''javascript
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####


'''javascript
...
```

#### <a name="apidoc.element.html-entities.Html5Entities.encodeNonUTF"></a>[function <span class="apidocSignatureSpan">html-entities.Html5Entities.</span>encodeNonUTF (str)](#apidoc.element.html-entities.Html5Entities.encodeNonUTF)
- description and source-code
```javascript
encodeNonUTF = function (str) {
   return new Html5Entities().encodeNonUTF(str);
}
```
- example usage
```shell
...

'''javascript
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####
...
```



# <a name="apidoc.module.html-entities.Html5Entities.prototype"></a>[module html-entities.Html5Entities.prototype](#apidoc.module.html-entities.Html5Entities.prototype)

#### <a name="apidoc.element.html-entities.Html5Entities.prototype.decode"></a>[function <span class="apidocSignatureSpan">html-entities.Html5Entities.prototype.</span>decode (str)](#apidoc.element.html-entities.Html5Entities.prototype.decode)
- description and source-code
```javascript
decode = function (str) {
    if (str.length === 0) {
        return '';
    }
    return str.replace(/&(#?[\w\d]+);?/g, function(s, entity) {
        var chr;
        if (entity.charAt(0) === "#") {
            var code = entity.charAt(1) === 'x' ?
                parseInt(entity.substr(2).toLowerCase(), 16) :
                parseInt(entity.substr(1));

            if (!(isNaN(code) || code < -32768 || code > 65535)) {
                chr = String.fromCharCode(code);
            }
        } else {
            chr = alphaIndex[entity];
        }
        return chr || s;
    });
}
```
- example usage
```shell
...
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####


'''javascript
var Entities = require('html-entities').AllHtmlEntities;
...
```

#### <a name="apidoc.element.html-entities.Html5Entities.prototype.encode"></a>[function <span class="apidocSignatureSpan">html-entities.Html5Entities.prototype.</span>encode (str)](#apidoc.element.html-entities.Html5Entities.prototype.encode)
- description and source-code
```javascript
encode = function (str) {
    var strLength = str.length;
    if (strLength === 0) {
        return '';
    }
    var result = '';
    var i = 0;
    while (i < strLength) {
        var charInfo = charIndex[str.charCodeAt(i)];
        if (charInfo) {
            var alpha = charInfo[str.charCodeAt(i + 1)];
            if (alpha) {
                i++;
            } else {
                alpha = charInfo[''];
            }
            if (alpha) {
                result += "&" + alpha + ";";
                i++;
                continue;
            }
        }
        result += str.charAt(i);
        i++;
    }
    return result;
}
```
- example usage
```shell
...
HTML validity and XSS attack prevention you can achieve from XmlEntities class.

'''javascript
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####
...
```

#### <a name="apidoc.element.html-entities.Html5Entities.prototype.encodeNonASCII"></a>[function <span class="apidocSignatureSpan">html-entities.Html5Entities.prototype.</span>encodeNonASCII (str)](#apidoc.element.html-entities.Html5Entities.prototype.encodeNonASCII)
- description and source-code
```javascript
encodeNonASCII = function (str) {
    var strLength = str.length;
    if (strLength === 0) {
        return '';
    }
    var result = '';
    var i = 0;
    while (i < strLength) {
        var c = str.charCodeAt(i);
        if (c <= 255) {
            result += str[i++];
            continue;
        }
        result += '&#' + c + ';';
        i++
    }
    return result;
}
```
- example usage
```shell
...
'''javascript
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####


'''javascript
...
```

#### <a name="apidoc.element.html-entities.Html5Entities.prototype.encodeNonUTF"></a>[function <span class="apidocSignatureSpan">html-entities.Html5Entities.prototype.</span>encodeNonUTF (str)](#apidoc.element.html-entities.Html5Entities.prototype.encodeNonUTF)
- description and source-code
```javascript
encodeNonUTF = function (str) {
    var strLength = str.length;
    if (strLength === 0) {
        return '';
    }
    var result = '';
    var i = 0;
    while (i < strLength) {
        var c = str.charCodeAt(i);
        var charInfo = charIndex[c];
        if (charInfo) {
            var alpha = charInfo[str.charCodeAt(i + 1)];
            if (alpha) {
                i++;
            } else {
                alpha = charInfo[''];
            }
            if (alpha) {
                result += "&" + alpha + ";";
                i++;
                continue;
            }
        }
        if (c < 32 || c > 126) {
            result += '&#' + c + ';';
        } else {
            result += str.charAt(i);
        }
        i++;
    }
    return result;
}
```
- example usage
```shell
...

'''javascript
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####
...
```



# <a name="apidoc.module.html-entities.XmlEntities"></a>[module html-entities.XmlEntities](#apidoc.module.html-entities.XmlEntities)

#### <a name="apidoc.element.html-entities.XmlEntities.XmlEntities"></a>[function <span class="apidocSignatureSpan">html-entities.</span>XmlEntities ()](#apidoc.element.html-entities.XmlEntities.XmlEntities)
- description and source-code
```javascript
function XmlEntities() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.html-entities.XmlEntities.decode"></a>[function <span class="apidocSignatureSpan">html-entities.XmlEntities.</span>decode (str)](#apidoc.element.html-entities.XmlEntities.decode)
- description and source-code
```javascript
decode = function (str) {
   return new XmlEntities().decode(str);
}
```
- example usage
```shell
...
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####


'''javascript
var Entities = require('html-entities').AllHtmlEntities;
...
```

#### <a name="apidoc.element.html-entities.XmlEntities.encode"></a>[function <span class="apidocSignatureSpan">html-entities.XmlEntities.</span>encode (str)](#apidoc.element.html-entities.XmlEntities.encode)
- description and source-code
```javascript
encode = function (str) {
   return new XmlEntities().encode(str);
}
```
- example usage
```shell
...
HTML validity and XSS attack prevention you can achieve from XmlEntities class.

'''javascript
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####
...
```

#### <a name="apidoc.element.html-entities.XmlEntities.encodeNonASCII"></a>[function <span class="apidocSignatureSpan">html-entities.XmlEntities.</span>encodeNonASCII (str)](#apidoc.element.html-entities.XmlEntities.encodeNonASCII)
- description and source-code
```javascript
encodeNonASCII = function (str) {
   return new XmlEntities().encodeNonASCII(str);
}
```
- example usage
```shell
...
'''javascript
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####


'''javascript
...
```

#### <a name="apidoc.element.html-entities.XmlEntities.encodeNonUTF"></a>[function <span class="apidocSignatureSpan">html-entities.XmlEntities.</span>encodeNonUTF (str)](#apidoc.element.html-entities.XmlEntities.encodeNonUTF)
- description and source-code
```javascript
encodeNonUTF = function (str) {
   return new XmlEntities().encodeNonUTF(str);
}
```
- example usage
```shell
...

'''javascript
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####
...
```



# <a name="apidoc.module.html-entities.XmlEntities.prototype"></a>[module html-entities.XmlEntities.prototype](#apidoc.module.html-entities.XmlEntities.prototype)

#### <a name="apidoc.element.html-entities.XmlEntities.prototype.decode"></a>[function <span class="apidocSignatureSpan">html-entities.XmlEntities.prototype.</span>decode (str)](#apidoc.element.html-entities.XmlEntities.prototype.decode)
- description and source-code
```javascript
decode = function (str) {
    if (str.length === 0) {
        return '';
    }
    return str.replace(/&#?[0-9a-zA-Z]+;?/g, function(s) {
        if (s.charAt(1) === '#') {
            var code = s.charAt(2).toLowerCase() === 'x' ?
                parseInt(s.substr(3), 16) :
                parseInt(s.substr(2));

            if (isNaN(code) || code < -32768 || code > 65535) {
                return '';
            }
            return String.fromCharCode(code);
        }
        return ALPHA_INDEX[s] || s;
    });
}
```
- example usage
```shell
...
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####


'''javascript
var Entities = require('html-entities').AllHtmlEntities;
...
```

#### <a name="apidoc.element.html-entities.XmlEntities.prototype.encode"></a>[function <span class="apidocSignatureSpan">html-entities.XmlEntities.prototype.</span>encode (str)](#apidoc.element.html-entities.XmlEntities.prototype.encode)
- description and source-code
```javascript
encode = function (str) {
    if (str.length === 0) {
        return '';
    }
    return str.replace(/<|>|"|'|&/g, function(s) {
        return CHAR_S_INDEX[s];
    });
}
```
- example usage
```shell
...
HTML validity and XSS attack prevention you can achieve from XmlEntities class.

'''javascript
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####
...
```

#### <a name="apidoc.element.html-entities.XmlEntities.prototype.encodeNonASCII"></a>[function <span class="apidocSignatureSpan">html-entities.XmlEntities.prototype.</span>encodeNonASCII (str)](#apidoc.element.html-entities.XmlEntities.prototype.encodeNonASCII)
- description and source-code
```javascript
encodeNonASCII = function (str) {
    var strLenght = str.length;
    if (strLenght === 0) {
        return '';
    }
    var result = '';
    var i = 0;
    while (i < strLenght) {
        var c = str.charCodeAt(i);
        if (c <= 255) {
            result += str[i++];
            continue;
        }
        result += '&#' + c + ';';
        i++;
    }
    return result;
}
```
- example usage
```shell
...
'''javascript
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####


'''javascript
...
```

#### <a name="apidoc.element.html-entities.XmlEntities.prototype.encodeNonUTF"></a>[function <span class="apidocSignatureSpan">html-entities.XmlEntities.prototype.</span>encodeNonUTF (str)](#apidoc.element.html-entities.XmlEntities.prototype.encodeNonUTF)
- description and source-code
```javascript
encodeNonUTF = function (str) {
    var strLength = str.length;
    if (strLength === 0) {
        return '';
    }
    var result = '';
    var i = 0;
    while (i < strLength) {
        var c = str.charCodeAt(i);
        var alpha = CHAR_INDEX[c];
        if (alpha) {
            result += "&" + alpha + ";";
            i++;
            continue;
        }
        if (c < 32 || c > 126) {
            result += '&#' + c + ';';
        } else {
            result += str.charAt(i);
        }
        i++;
    }
    return result;
}
```
- example usage
```shell
...

'''javascript
var Entities = require('html-entities').XmlEntities;

entities = new Entities();

console.log(entities.encode('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;©®
console.log(entities.encodeNonUTF('<>"\'&©®')); // &lt;&gt;&quot;&apos;&amp;&#169;&#174;
console.log(entities.encodeNonASCII('<>"\'&©®')); // <>"\'&©®
console.log(entities.decode('&lt;&gt;&quot;&apos;&amp;&copy;&reg;&#8710;')); // <>"'&&copy;&reg;∆
'''

####All HTML entities encoding/decoding####
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
