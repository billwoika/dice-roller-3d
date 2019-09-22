# Dice Roller
[![npm package](https://img.shields.io/npm/v/roll-a-die.svg?style=flat-square)](https://www.npmjs.org/package/dice-roller3-d) 

Simple 3D dice roll animator using CSS3 Animation.


## Vanilla JS
Copy dist/dice-roller.js into your library folder
Load it into your HTML script
```
<script type="text/javascript" src="path/to/dice-roller.js"></script>
```

Call the method with its options.
```
{
  element: Element;
  numberOfDice: number;
  delay: number;
  callback: Function;
  values: number[];
}

diceRoller(options);
```

## With npm (and CommonJS builder)
Install with npm.
```
npm install --save dice-roller-3d
```

import the library

ES5
```
const diceRoller = require('dice-roller-3d');
```

ES6
```
import diceRoller from 'dice-roller-3d';
```

Call the method
```
const result = diceRoller({ element, numberOfDice: 2, callback});
const result = diceRoller({ element, numberOfDice: 2, callback, noSound: true});
const result = diceRoller({ element, numberOfDice: 2, callback, delay: 1000});
const result = diceRoller({ element, numberOfDice: 2, callback, values: [3, 4]});
```

## Parameter Definitions

* `element`: The element to render die animation on. Type: HTMLElement
* `numberOfDice`: The number of dice to use.` Type: number
* `callback`: Called when animation is finished. Returns an array of the values from throw. Type: Function
* `noSound`: Roll the die without sound (Optional). Type: boolean
* `delay`: Time in milliseconds to delay before removing animations (Optional). Type: number
* `values`: Values to show on die face. When provided, it overrides library genrated values. (Optional). Type: Array of numbers

## Thanks
* (Sound Effect)
   * http://commons.nicovideo.jp/material/nc93322
* Forked from: https://github.com/chukwumaijem/roll-a-die

## License
MIT License
