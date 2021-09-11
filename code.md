# JS Code

10.09.2021
### MakeUpperCase
```
function makeUpperCase(str) {
  let string = str.toUpperCase()
  return string
}
```
--------
### Grasshopper - Summation
```
var summation = function (num) {
    let totalSum = 0
    for(let i = 0; i <= num; i++) {
        totalSum = i + totalSum
    }
    return totalSum
}
```
--------

11.09.2021
### Condition
```
let boolOne = 5 > 3;
let boolTwo = 5 < 3;

if(boolOne){
  console.log("That's right");
  }else{
  console.log("That's wrong");
}
```
--------
### Roll Dice 
```
function rollDice(num1, num2){
let response;
if(num1 > num2){
  response = "Number 1 wins";
  }else if(num1 == num2){
  response = "Tie game";
  }else{
  response = "Number 2 wins";
}
return response;
}

rollDice(5, 7);
rollDice(9, 7);
```
-------

### Condition (Message)
```
let message = (5 == 5) ? 'TRUE' : 'FALSE';
console.log(message);
```
----------

### Randon Number (from 0 to 5)

```
Math.floor(Math.random() * 5);
```
------------

### Randon Number (from 1 to 5)

```
Math.floor(Math.random() * 5) + 1;
```
-----------
### Code (Unresolved)
```
let a = randomNum(5);
let b = randomNum(6);

function randomNum(val){
	return Math.floor(Math.random() * val) + 1;
}

function rollDice(num1, num2){
    let response;
if(num1 > num2){
  response = "Number 1 wins";
  }else if(num1 == num2){
  response = "Tie game";
  }else{
  response = "Number 2 wins";
}
return response;
}

let message = rollDice(a, b);
console.log(a + " vs " + b + " " + message);
```
From - Class: JavaScript Math Object, Course: Learn JavaScript. Quick Course for Beginners, Platform: BitDegree.
------------
