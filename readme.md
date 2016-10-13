Scroll area component
==============

[![Build Status](https://img.shields.io/travis/magsdk/component-scroll-area.svg?style=flat-square)](https://travis-ci.org/magsdk/component-scroll-area)
[![NPM version](https://img.shields.io/npm/v/mag-component-scroll-area.svg?style=flat-square)](https://www.npmjs.com/package/mag-component-scroll-area)
[![Dependencies Status](https://img.shields.io/david/spasdk/component-scroll-area.svg?style=flat-square)](https://david-dm.org/spasdk/component-scroll-area)
[![Gitter](https://img.shields.io/badge/gitter-join%20chat-blue.svg?style=flat-square)](https://gitter.im/DarkPark/spasdk)


Scroll area is a component to build user interface, an instance of [Component](https://github.com/spasdk/component) module.


## Installation ##

```bash
npm install mag-component-scroll-area
```


## Usage ##

Add the constructor to the scope:

```js
var ScrollArea = require('mag-component-scroll-area');
```

Specific properties:

NAME        | TYPE      | DEFAULT VALUE | DESCRIPTION                               |
------------|-----------|---------------|-------------------------------------------|
step        | number    | 5             | Step to scroll area in % of screen height |
realHeight  | number    | 0             | Real height of scroll area                |
viewHeight  | number    | 0             | Visible height of area                    |
topPosition | number    | 0             | Top position of scroll container          |
scroll      | ScrollBar | null          | Associated [ScrollBar](https://github.com/stbsdk/component-scrollbar) component link       |

Create scroll area instance:

```js
var scrollArea = new ScrollArea({
    scroll: scrollBar,
    step: 5
});
```

Add scrollable content to the scroll area:

```js
scrollArea.$body.innerText = 'Some long long long text to scroll..........';
```

Re-init of the component with new data:

```js
scrollArea.init();
```


## Development mode ##

> There is a global var `DEVELOP` which activates additional consistency checks and protection logic not available in release mode.


## Contribution ##

If you have any problem or suggestion please open an issue [here](https://github.com/spasdk/component-scroll-area/issues).
Pull requests are welcomed with respect to the [JavaScript Code Style](https://github.com/DarkPark/jscs).


## License ##

`mag-component-scroll-area` is released under the [MIT License](license.md).
