
# device

  Simple device detection

## Installation

  Install with [component(1)](http://component.io):

    $ component install slajax/device

## API

by default it parses `navigator.userAgent`...

```javascript
  var d = require('device')();
  d.getDevice(); // desktop
  d.is_desktop; // true
  d.is_mobile; // false
  d.is_phone; // false
  d.is_tablet; // false;
  d.is_tv; // false
  d.is_bot; // false
```

override `navigator.userAgent` like so:

```javascript
  var d = require('device')('My Custom User Agent');
  d.getDevice();
```


## License

(The MIT License)

Copyright (c) 2013 Kyle Campbell <mail@slajax.com>, inspiration and getDevice inspired by [express-device](https://github.com/rguerreiro/express-device)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
