# rpncs
[![Build Status](https://travis-ci.org/TsutomuNakamura/rpncc.svg?branch=master)](https://travis-ci.org/TsutomuNakamura/rpncs) 
[![npm](https://img.shields.io/npm/v/rpncs.svg)](https://npmjs.com/package/rpncs) 
[![GitHub license](https://img.shields.io/github/license/TsutomuNakamura/rpncs.svg)](https://github.com/TsutomuNakamura/rpncs)
[![npm total downloads](https://img.shields.io/npm/dt/rpncs.svg)](https://github.com/TsutomuNakamura/rpncs)

This is a program for Reverse Polish notation utility.
It converts or calculates a expressions to Reverse Polish notation.

## Use examples
First, install this module in your project.
```console
$ npm install rpncs
```

Import this module in your source code and call like below.
```javascript
var Rpn = require('rpncs');
var rpn = new Rpn();

console.log(rpn.convert(["1", "+", "2", "*", "3"]));     // -> [ '1', '2', '3', '*', '+' ]
console.log(rpn.calculate([ '1', '2', '3', '*', '+' ])); // -> 7
console.log(rpn.revert([ '1', '2', '3', '*', '+' ]));    // -> ["1", "+", "2", "*", "3"]
```

## Testing
rpncs uses ava for testing. You can run test cases by installing dependencies then run "npm test" command.
```console
$ npm install
$ npm test
```

## License
This software is released under the MIT License, see LICENSE.txt.
