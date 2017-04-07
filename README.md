# api documentation for  [charm (v1.0.2)](https://github.com/substack/node-charm#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-charm.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-charm) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-charm.svg)](https://travis-ci.org/npmdoc/node-npmdoc-charm)
#### ansi control sequences for terminal cursor hopping and colors

[![NPM](https://nodei.co/npm/charm.png?downloads=true)](https://www.npmjs.com/package/charm)

[![apidoc](https://npmdoc.github.io/node-npmdoc-charm/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-charm%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-charm/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-charm/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-charm/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "James Halliday",
        "email": "mail@substack.net",
        "url": "http://substack.net"
    },
    "bugs": {
        "url": "https://github.com/substack/node-charm/issues"
    },
    "dependencies": {
        "inherits": "^2.0.1"
    },
    "description": "ansi control sequences for terminal cursor hopping and colors",
    "devDependencies": {},
    "directories": {
        "lib": ".",
        "example": "example",
        "test": "test"
    },
    "dist": {
        "shasum": "8add367153a6d9a581331052c4090991da995e35",
        "tarball": "https://registry.npmjs.org/charm/-/charm-1.0.2.tgz"
    },
    "engine": {
        "node": ">=0.4"
    },
    "gitHead": "1f68b8a4cf3375f15dd01e2a0f7318ee37c58c75",
    "homepage": "https://github.com/substack/node-charm#readme",
    "keywords": [
        "terminal",
        "ansi",
        "cursor",
        "color",
        "console",
        "control",
        "escape",
        "sequence"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "noffle",
            "email": "stephen.whitmore@gmail.com"
        },
        {
            "name": "substack",
            "email": "substack@gmail.com"
        }
    ],
    "name": "charm",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/substack/node-charm.git"
    },
    "scripts": {},
    "version": "1.0.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module charm](#apidoc.module.charm)
1.  [function <span class="apidocSignatureSpan">charm.</span>Charm ()](#apidoc.element.charm.Charm)
1.  [function <span class="apidocSignatureSpan">charm.</span>encode (xs)](#apidoc.element.charm.encode)
1.  [function <span class="apidocSignatureSpan">charm.</span>extractCodes (buf)](#apidoc.element.charm.extractCodes)
1.  object <span class="apidocSignatureSpan">charm.</span>Charm.prototype

#### [module charm.Charm](#apidoc.module.charm.Charm)
1.  [function <span class="apidocSignatureSpan">charm.</span>Charm ()](#apidoc.element.charm.Charm.Charm)
1.  [function <span class="apidocSignatureSpan">charm.Charm.</span>super_ ()](#apidoc.element.charm.Charm.super_)

#### [module charm.Charm.prototype](#apidoc.module.charm.Charm.prototype)
1.  [function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>background (color)](#apidoc.element.charm.Charm.prototype.background)
1.  [function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>column (x)](#apidoc.element.charm.Charm.prototype.column)
1.  [function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>cursor (visible)](#apidoc.element.charm.Charm.prototype.cursor)
1.  [function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>delete (s, n)](#apidoc.element.charm.Charm.prototype.delete)
1.  [function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>destroy ()](#apidoc.element.charm.Charm.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>display (attr)](#apidoc.element.charm.Charm.prototype.display)
1.  [function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>down (y)](#apidoc.element.charm.Charm.prototype.down)
1.  [function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>end (buf)](#apidoc.element.charm.Charm.prototype.end)
1.  [function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>erase (s)](#apidoc.element.charm.Charm.prototype.erase)
1.  [function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>foreground (color)](#apidoc.element.charm.Charm.prototype.foreground)
1.  [function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>insert (mode, n)](#apidoc.element.charm.Charm.prototype.insert)
1.  [function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>left (x)](#apidoc.element.charm.Charm.prototype.left)
1.  [function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>move (x, y)](#apidoc.element.charm.Charm.prototype.move)
1.  [function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>pop (withAttributes)](#apidoc.element.charm.Charm.prototype.pop)
1.  [function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>position (x, y)](#apidoc.element.charm.Charm.prototype.position)
1.  [function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>push (withAttributes)](#apidoc.element.charm.Charm.prototype.push)
1.  [function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>reset (cb)](#apidoc.element.charm.Charm.prototype.reset)
1.  [function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>right (x)](#apidoc.element.charm.Charm.prototype.right)
1.  [function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>up (y)](#apidoc.element.charm.Charm.prototype.up)
1.  [function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>write (buf)](#apidoc.element.charm.Charm.prototype.write)

#### [module charm.encode](#apidoc.module.charm.encode)
1.  [function <span class="apidocSignatureSpan">charm.</span>encode (xs)](#apidoc.element.charm.encode.encode)
1.  [function <span class="apidocSignatureSpan">charm.encode.</span>ord (c)](#apidoc.element.charm.encode.ord)



# <a name="apidoc.module.charm"></a>[module charm](#apidoc.module.charm)

#### <a name="apidoc.element.charm.Charm"></a>[function <span class="apidocSignatureSpan">charm.</span>Charm ()](#apidoc.element.charm.Charm)
- description and source-code
```javascript
function Charm() {
    this.writable = true;
    this.readable = true;
    this.pending = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.charm.encode"></a>[function <span class="apidocSignatureSpan">charm.</span>encode (xs)](#apidoc.element.charm.encode)
- description and source-code
```javascript
encode = function (xs) {
    function bytes (s) {
        if (typeof s === 'string') {
            return s.split('').map(ord);
        }
        else if (Array.isArray(s)) {
            return s.reduce(function (acc, c) {
                return acc.concat(bytes(c));
            }, []);
        }
    }

    return new Buffer([ 0x1b ].concat(bytes(xs)));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.charm.extractCodes"></a>[function <span class="apidocSignatureSpan">charm.</span>extractCodes (buf)](#apidoc.element.charm.extractCodes)
- description and source-code
```javascript
extractCodes = function (buf) {
    var codes = [];
    var start = -1;

    for (var i = 0; i < buf.length; i++) {
        if (buf[i] === 27) {
            if (start >= 0) codes.push(buf.slice(start, i));
            start = i;
        }
        else if (start >= 0 && i === buf.length - 1) {
            codes.push(buf.slice(start));
        }
    }

    return codes;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.charm.Charm"></a>[module charm.Charm](#apidoc.module.charm.Charm)

#### <a name="apidoc.element.charm.Charm.Charm"></a>[function <span class="apidocSignatureSpan">charm.</span>Charm ()](#apidoc.element.charm.Charm.Charm)
- description and source-code
```javascript
function Charm() {
    this.writable = true;
    this.readable = true;
    this.pending = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.charm.Charm.super_"></a>[function <span class="apidocSignatureSpan">charm.Charm.</span>super_ ()](#apidoc.element.charm.Charm.super_)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.charm.Charm.prototype"></a>[module charm.Charm.prototype](#apidoc.module.charm.Charm.prototype)

#### <a name="apidoc.element.charm.Charm.prototype.background"></a>[function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>background (color)](#apidoc.element.charm.Charm.prototype.background)
- description and source-code
```javascript
background = function (color) {
    if (typeof color === 'number') {
        if (color < 0 || color >= 256) {
            this.emit('error', new Error('Color out of range: ' + color));
        }
        this.write(encode('[48;5;' + color + 'm'));
    }
    else {
        var c = {
          black : 40,
          red : 41,
          green : 42,
          yellow : 43,
          blue : 44,
          magenta : 45,
          cyan : 46,
          white : 47
        }[color.toLowerCase()];

        if (!c) this.emit('error', new Error('Unknown color: ' + color));
        this.write(encode('[' + c + 'm'));
    }
    return this;
}
```
- example usage
```shell
...
* cyan
* magenta
* black
* white

or 'color' can be an integer from 0 to 255, inclusive.

charm.background(color)
-----------------------

Set the background color with the string 'color', which can be:

* red
* yellow
* green
...
```

#### <a name="apidoc.element.charm.Charm.prototype.column"></a>[function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>column (x)](#apidoc.element.charm.Charm.prototype.column)
- description and source-code
```javascript
column = function (x) {
    this.write(encode('[' + Math.floor(x) + 'G'));
    return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.charm.Charm.prototype.cursor"></a>[function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>cursor (visible)](#apidoc.element.charm.Charm.prototype.cursor)
- description and source-code
```javascript
cursor = function (visible) {
    this.write(encode(visible ? '[?25h' : '[?25l'));
    return this;
}
```
- example usage
```shell
...
* cyan
* magenta
* black
* white

or 'color' can be an integer from 0 to 255, inclusive.

charm.cursor(visible)
---------------------

Set the cursor visibility with a boolean 'visible'.

install
=======
...
```

#### <a name="apidoc.element.charm.Charm.prototype.delete"></a>[function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>delete (s, n)](#apidoc.element.charm.Charm.prototype.delete)
- description and source-code
```javascript
delete = function (s, n) {
    n = n || 1

    if (s === 'line') {
        this.write(encode('[' + n + 'M'));
    }
    else if (s === 'char') {
        this.write(encode('[' + n + 'M'));
    }
    else {
        this.emit('error', new Error('Unknown delete type: ' + s));
    }
    return this;
}
```
- example usage
```shell
...
* end - erase from the cursor to the end of the line
* start - erase from the cursor to the start of the line
* line - erase the current line
* down - erase everything below the current line
* up - erase everything above the current line
* screen - erase the entire screen

charm.delete(mode, n)
---------------------
Delete ''line'' or ''char''s. 'delete' differs from erase
because it does not write over the deleted characters with whitesapce,
but instead removes the deleted space.

'mode' can be ''line'' or ''char''. 'n' is the number of items to be deleted.
'n' must be a positive integer.
...
```

#### <a name="apidoc.element.charm.Charm.prototype.destroy"></a>[function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>destroy ()](#apidoc.element.charm.Charm.prototype.destroy)
- description and source-code
```javascript
destroy = function () {
    this.end();
}
```
- example usage
```shell
...
You can 'pipe()' to and from the 'charm' object you get back.

charm.reset()
-------------

Reset the entire screen, like the /usr/bin/reset command.

charm.destroy(), charm.end()
----------------------------

Emit an '"end"' event downstream.

charm.write(msg)
----------------
...
```

#### <a name="apidoc.element.charm.Charm.prototype.display"></a>[function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>display (attr)](#apidoc.element.charm.Charm.prototype.display)
- description and source-code
```javascript
display = function (attr) {
    var c = {
        reset : 0,
        bright : 1,
        dim : 2,
        underscore : 4,
        blink : 5,
        reverse : 7,
        hidden : 8
    }[attr];
    if (c === undefined) {
        this.emit('error', new Error('Unknown attribute: ' + attr));
    }
    this.write(encode('[' + c + 'm'));
    return this;
}
```
- example usage
```shell
...

charm.insert(mode, n)
---------------------

Insert space into the terminal. 'insert' is the opposite of' delete',
and the arguments are the same.

charm.display(attr)
-------------------

Set the display mode with the string 'attr'.

'attr' can be:

* reset
...
```

#### <a name="apidoc.element.charm.Charm.prototype.down"></a>[function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>down (y)](#apidoc.element.charm.Charm.prototype.down)
- description and source-code
```javascript
down = function (y) {
    if (y === undefined) y = 1;
    this.write(encode('[' + Math.floor(y) + 'B'));
    return this;
}
```
- example usage
```shell
...
Move the cursor position by the relative coordinates 'x, y'.

charm.up(y)
-----------

Move the cursor up by 'y' rows.

charm.down(y)
-------------

Move the cursor down by 'y' rows.

charm.left(x)
-------------
...
```

#### <a name="apidoc.element.charm.Charm.prototype.end"></a>[function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>end (buf)](#apidoc.element.charm.Charm.prototype.end)
- description and source-code
```javascript
end = function (buf) {
    if (buf) this.write(buf);
    this.emit('end');
}
```
- example usage
```shell
...
You can 'pipe()' to and from the 'charm' object you get back.

charm.reset()
-------------

Reset the entire screen, like the /usr/bin/reset command.

charm.destroy(), charm.end()
----------------------------

Emit an '"end"' event downstream.

charm.write(msg)
----------------
...
```

#### <a name="apidoc.element.charm.Charm.prototype.erase"></a>[function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>erase (s)](#apidoc.element.charm.Charm.prototype.erase)
- description and source-code
```javascript
erase = function (s) {
    if (s === 'end' || s === '$') {
        this.write(encode('[K'));
    }
    else if (s === 'start' || s === '^') {
        this.write(encode('[1K'));
    }
    else if (s === 'line') {
        this.write(encode('[2K'));
    }
    else if (s === 'down') {
        this.write(encode('[J'));
    }
    else if (s === 'up') {
        this.write(encode('[1J'));
    }
    else if (s === 'screen') {
        this.write(encode('[1J'));
    }
    else {
        this.emit('error', new Error('Unknown erase type: ' + s));
    }
    return this;
}
```
- example usage
```shell
...
Push the cursor state and optionally the attribute state.

charm.pop(withAttributes=false)
-------------------------------

Pop the cursor state and optionally the attribute state.

charm.erase(s)
--------------

Erase a region defined by the string 's'.

's' can be:

* end - erase from the cursor to the end of the line
...
```

#### <a name="apidoc.element.charm.Charm.prototype.foreground"></a>[function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>foreground (color)](#apidoc.element.charm.Charm.prototype.foreground)
- description and source-code
```javascript
foreground = function (color) {
    if (typeof color === 'number') {
        if (color < 0 || color >= 256) {
            this.emit('error', new Error('Color out of range: ' + color));
        }
        this.write(encode('[38;5;' + color + 'm'));
    }
    else {
        var c = {
            black : 30,
            red : 31,
            green : 32,
            yellow : 33,
            blue : 34,
            magenta : 35,
            cyan : 36,
            white : 37
        }[color.toLowerCase()];

        if (!c) this.emit('error', new Error('Unknown color: ' + color));
        this.write(encode('[' + c + 'm'));
    }
    return this;
}
```
- example usage
```shell
...
var iv = setInterval(function () {
var y = 0, dy = 1;
for (var i = 0; i < 40; i++) {
    var color = colors[(i + offset) % colors.length];
    var c = text[(i + offset) % text.length];
    charm
        .move(1, dy)
        .foreground(color)
        .write(c)
    ;
    y += dy;
    if (y <= 0 || y >= 5) dy *= -1;
}
charm.position(0, 1);
offset ++;
...
```

#### <a name="apidoc.element.charm.Charm.prototype.insert"></a>[function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>insert (mode, n)](#apidoc.element.charm.Charm.prototype.insert)
- description and source-code
```javascript
insert = function (mode, n) {
    n = n || 1

    if(mode === true) {
        this.write(encode('[4h'));
    }
    else if (mode === false) {
        this.write(encode('[l'));
    }
    else if (mode === 'line') {
        this.write(encode('[' + n + 'L'));
    }
    else if (mode === 'char') {
        this.write(encode('[' + n + '@'));
    }
    else {
        this.emit('error', new Error('Unknown delete type: ' + s));
    }
    return this;
}
```
- example usage
```shell
...
but instead removes the deleted space.

'mode' can be ''line'' or ''char''. 'n' is the number of items to be deleted.
'n' must be a positive integer.

The cursor position is not updated.

charm.insert(mode, n)
---------------------

Insert space into the terminal. 'insert' is the opposite of' delete',
and the arguments are the same.

charm.display(attr)
-------------------
...
```

#### <a name="apidoc.element.charm.Charm.prototype.left"></a>[function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>left (x)](#apidoc.element.charm.Charm.prototype.left)
- description and source-code
```javascript
left = function (x) {
    if (x === undefined) x = 1;
    this.write(encode('[' + Math.floor(x) + 'D'));
    return this;
}
```
- example usage
```shell
...
Move the cursor up by 'y' rows.

charm.down(y)
-------------

Move the cursor down by 'y' rows.

charm.left(x)
-------------

Move the cursor left by 'x' columns.

charm.right(x)
--------------
...
```

#### <a name="apidoc.element.charm.Charm.prototype.move"></a>[function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>move (x, y)](#apidoc.element.charm.Charm.prototype.move)
- description and source-code
```javascript
move = function (x, y) {
    // set relative coordinates
    var bufs = [];

    if (y < 0) this.up(-y)
    else if (y > 0) this.down(y)

    if (x > 0) this.right(x)
    else if (x < 0) this.left(-x)

    return this;
}
```
- example usage
```shell
...
var offset = 0;
var iv = setInterval(function () {
var y = 0, dy = 1;
for (var i = 0; i < 40; i++) {
    var color = colors[(i + offset) % colors.length];
    var c = text[(i + offset) % text.length];
    charm
        .move(1, dy)
        .foreground(color)
        .write(c)
    ;
    y += dy;
    if (y <= 0 || y >= 5) dy *= -1;
}
charm.position(0, 1);
...
```

#### <a name="apidoc.element.charm.Charm.prototype.pop"></a>[function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>pop (withAttributes)](#apidoc.element.charm.Charm.prototype.pop)
- description and source-code
```javascript
pop = function (withAttributes) {
    this.write(encode(withAttributes ? '8' : '[u'));
    return this;
}
```
- example usage
```shell
...
Move the cursor right by 'x' columns.

charm.push(withAttributes=false)
--------------------------------

Push the cursor state and optionally the attribute state.

charm.pop(withAttributes=false)
-------------------------------

Pop the cursor state and optionally the attribute state.

charm.erase(s)
--------------
...
```

#### <a name="apidoc.element.charm.Charm.prototype.position"></a>[function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>position (x, y)](#apidoc.element.charm.Charm.prototype.position)
- description and source-code
```javascript
position = function (x, y) {
    // get/set absolute coordinates
    if (typeof x === 'function') {
        var cb = x;
        this.pending.push(function (buf) {
            if (buf[0] === 27 && buf[1] === encode.ord('[')
            && buf[buf.length-1] === encode.ord('R')) {
                var pos = buf.toString()
                    .slice(2,-1)
                    .split(';')
                    .map(Number)
                ;
                cb(pos[1], pos[0]);
                return true;
            }
        });
        this.write(encode('[6n'));
    }
    else {
        this.write(encode(
            '[' + Math.floor(y) + ';' + Math.floor(x) + 'f'
        ));
    }
    return this;
}
```
- example usage
```shell
...
            .move(1, dy)
            .foreground(color)
            .write(c)
        ;
        y += dy;
        if (y <= 0 || y >= 5) dy *= -1;
    }
    charm.position(0, 1);
    offset ++;
}, 150);
''''

events
======
...
```

#### <a name="apidoc.element.charm.Charm.prototype.push"></a>[function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>push (withAttributes)](#apidoc.element.charm.Charm.prototype.push)
- description and source-code
```javascript
push = function (withAttributes) {
    this.write(encode(withAttributes ? '7' : '[s'));
    return this;
}
```
- example usage
```shell
...
Move the cursor left by 'x' columns.

charm.right(x)
--------------

Move the cursor right by 'x' columns.

charm.push(withAttributes=false)
--------------------------------

Push the cursor state and optionally the attribute state.

charm.pop(withAttributes=false)
-------------------------------
...
```

#### <a name="apidoc.element.charm.Charm.prototype.reset"></a>[function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>reset (cb)](#apidoc.element.charm.Charm.prototype.reset)
- description and source-code
```javascript
reset = function (cb) {
    // resets the screen on iTerm, which appears
    // to lack support for the reset character.
    this.write(encode('[0m'));
    this.write(encode('[2J'));

    this.write(encode('c'));
    return this;
}
```
- example usage
```shell
...

lucky
-----

''''javascript
var charm = require('charm')();
charm.pipe(process.stdout);
charm.reset();

var colors = [ 'red', 'cyan', 'yellow', 'green', 'blue' ];
var text = 'Always after me lucky charms.';

var offset = 0;
var iv = setInterval(function () {
var y = 0, dy = 1;
...
```

#### <a name="apidoc.element.charm.Charm.prototype.right"></a>[function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>right (x)](#apidoc.element.charm.Charm.prototype.right)
- description and source-code
```javascript
right = function (x) {
    if (x === undefined) x = 1;
    this.write(encode('[' + Math.floor(x) + 'C'));
    return this;
}
```
- example usage
```shell
...
Move the cursor down by 'y' rows.

charm.left(x)
-------------

Move the cursor left by 'x' columns.

charm.right(x)
--------------

Move the cursor right by 'x' columns.

charm.push(withAttributes=false)
--------------------------------
...
```

#### <a name="apidoc.element.charm.Charm.prototype.up"></a>[function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>up (y)](#apidoc.element.charm.Charm.prototype.up)
- description and source-code
```javascript
up = function (y) {
    if (y === undefined) y = 1;
    this.write(encode('[' + Math.floor(y) + 'A'));
    return this;
}
```
- example usage
```shell
...
'cb(x, y)'.

charm.move(x, y)
----------------

Move the cursor position by the relative coordinates 'x, y'.

charm.up(y)
-----------

Move the cursor up by 'y' rows.

charm.down(y)
-------------
...
```

#### <a name="apidoc.element.charm.Charm.prototype.write"></a>[function <span class="apidocSignatureSpan">charm.Charm.prototype.</span>write (buf)](#apidoc.element.charm.Charm.prototype.write)
- description and source-code
```javascript
write = function (buf) {
    var self = this;

    if (self.pending.length) {
        var codes = extractCodes(buf);
        var matched = false;

        for (var i = 0; i < codes.length; i++) {
            for (var j = 0; j < self.pending.length; j++) {
                var cb = self.pending[j];
                if (cb(codes[i])) {
                    matched = true;
                    self.pending.splice(j, 1);
                    break;
                }
            }
        }

        if (matched) return;
    }

    if (buf.length === 1) {
        if (buf[0] === 3) self.emit('^C');
        if (buf[0] === 4) self.emit('^D');
    }

    self.emit('data', buf);

    return self;
}
```
- example usage
```shell
...
    var y = 0, dy = 1;
    for (var i = 0; i < 40; i++) {
        var color = colors[(i + offset) % colors.length];
        var c = text[(i + offset) % text.length];
        charm
            .move(1, dy)
            .foreground(color)
            .write(c)
        ;
        y += dy;
        if (y <= 0 || y >= 5) dy *= -1;
    }
    charm.position(0, 1);
    offset ++;
}, 150);
...
```



# <a name="apidoc.module.charm.encode"></a>[module charm.encode](#apidoc.module.charm.encode)

#### <a name="apidoc.element.charm.encode.encode"></a>[function <span class="apidocSignatureSpan">charm.</span>encode (xs)](#apidoc.element.charm.encode.encode)
- description and source-code
```javascript
encode = function (xs) {
    function bytes (s) {
        if (typeof s === 'string') {
            return s.split('').map(ord);
        }
        else if (Array.isArray(s)) {
            return s.reduce(function (acc, c) {
                return acc.concat(bytes(c));
            }, []);
        }
    }

    return new Buffer([ 0x1b ].concat(bytes(xs)));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.charm.encode.ord"></a>[function <span class="apidocSignatureSpan">charm.encode.</span>ord (c)](#apidoc.element.charm.encode.ord)
- description and source-code
```javascript
function ord(c) {
    return c.charCodeAt(0)
}
```
- example usage
```shell
...
};

Charm.prototype.position = function (x, y) {
// get/set absolute coordinates
if (typeof x === 'function') {
    var cb = x;
    this.pending.push(function (buf) {
        if (buf[0] === 27 && buf[1] === encode.ord('[')
        && buf[buf.length-1] === encode.ord('R')) {
            var pos = buf.toString()
                .slice(2,-1)
                .split(';')
                .map(Number)
            ;
            cb(pos[1], pos[0]);
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
