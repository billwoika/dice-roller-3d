# Roll A Die
[![npm package](https://img.shields.io/npm/v/roll-a-die.svg?style=flat-square)](https://www.npmjs.org/package/roll-a-die)  [![Build Status](https://img.shields.io/travis/chukwumaijem/roll-a-die.svg?style=flat-square)](https://travis-ci.com/chukwumaijem/roll-a-die.svg?branch=master)

Simple 3D dice roll animator by CSS3 Animation.


## Vanilla JS
[Demo](https://codepen.io/chukwuma-ezumezu/pen/qYKOGW)
Copy dist/roll-a-die.js into your library folder
Load it into your HTML script
```
<script type="text/javascript" src="path/to/roll-a-die.js"></script>
```
You can use the [UNPKG](https://unpkg.com) link `https://unpkg.com/roll-a-die@1.0.4/dist/roll-a-die.js`. Remember to update the package number to the most recent.

Call the method with its options.
```
rollADie({ element, numberDice: 2, callback});
```

## With npm (and CommonJS builder)
Install with npm.
```npm install --save roll-a-die```

Install with yarn.
```yarn add roll-a-die```

import the library

ES5
```const rollADie = require('roll-a-die');```

ES6
```import rollADie from 'roll-a-die';```

Call the method
```
rollADie({ element, numberDice: 2, callback});
rollADie({ element, numberDice: 2, callback, noSound: true});
rollADie({ element, numberDice: 2, callback, delay: 1000});
```

## Parameter Definitions

* `element`: The element to render die animation on.
* `numberDice`: The number of dice to use.`
* `callback`: Called when animation is finished. Returns an array of the values from throw.
* `noSound`: Roll the die without sound (Optional).
* `delay`: Time in milliseconds to delay before removing animations (Optional).

## Thanks
* (Sound Effect)
   * http://commons.nicovideo.jp/material/nc93322

## License
MIT License