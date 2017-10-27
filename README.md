# sudoku-solver-js

> Simple Sudoku solver in javascript.

Check out the [Demo](https://samirhodzic.github.io/sudoku-solver-js) to see it in action.

### How to use?

```bash
$ npm install sudoku-solver-js
```
**or** 
simply include `index.js` into your HTML file for browser usage.

Example usage:
```javascript
var SudokuSolver = require('sudoku-solver-js');
var puzzle = '001700509573024106800501002700295018009400305652800007465080071000159004908007053';

solver.solve(puzzle)
```
Output:
```javascript
'241768539573924186896531742734295618189476325652813497465382971327159864918647253'
```

### Options

```javascript
var SudokuSolver = require('sudoku-solver-js');
var puzzle = '001700509573024106800501002700295018009400305652800007465080071000159004908007053';

solver.solve(puzzle, { result: 'string' })

Result values: 
// string
'241768539573924186896531742734295618189476325652813497465382971327159864918647253'

// array
[2,4,1,7,6,8,5,3,9,5,7,3,9,2,4,1,8,6,8,9,6,5,3,1,7,4,2,7,3,4,2,9,5,6,1,8,1,8,9,4,7,6,3,2,5,6,5,2,8,1,3,4,9,7,4,6,5,3,8,2,9,7,1,3,2,7,1,5,9,8,6,4,9,1,8,6,4,7,2,5,3]

// chunks (by 9)
[[2,4,1,7,6,8,5,3,9],[5,7,3,9,2,4,1,8,6],[8,9,6,5,3,1,7,4,2],[7,3,4,2,9,5,6,1,8],[1,8,9,4,7,6,3,2,5],[6,5,2,8,1,3,4,9,7],[4,6,5,3,8,2,9,7,1],[3,2,7,1,5,9,8,6,4],[9,1,8,6,4,7,2,5,3]]
```
### Test

```bash
$ npm test
```
