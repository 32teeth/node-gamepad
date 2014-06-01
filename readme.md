# node-gamepad

> node-gamepad is a package for node that allows you to effortlessly interface your node applications with a variety of gamepad controllers.

## Installation

```js
npm install node-gamepad
```

## How to Use

Plug in a supported controller and run a variation of the code below:

### For PS3

```js
var GamePad = require( 'node-gamepad' );
var controller = new GamePad( 'ps3/dualshock3' );
controller.connect();

controller.on( 'up:press', function() {
    console.log( 'up' );
} );
controller.on( 'down:press', function() {
    console.log( 'down' );
} );
```

### For SNES

```js
var GamePad = require( 'node-gamepad' );
var controller = new GamePad( 'snes/tomee' );
controller.connect();

controller.on( 'up:press', function() {
    console.log( 'up' );
} );
controller.on( 'down:press', function() {
    console.log( 'down' );
} );
```

## License

The MIT License (MIT)

Copyright (c) 2014 Carl Danley

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.