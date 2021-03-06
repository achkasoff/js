# JS Code
29.09.2021
### If ... else (html)
```js
var course = 2;
if (course == 1) {
    document.write("<h1>HTML Tutorial</h1>");
} else if (course == 2) {
    document.write("<h1>CSS Tutorial</h1>");
} else {
    document.write("<h1>JavaScript Tutorial</h1>");
}
```
23.09.2021
### Function
```js
function fruitProcess(apples, oranges) {
//	console.log(apples, oranges);
	const juice = `Juice with ${apples} apples and ${oranges} oranges.`;
	return juice;
}
fruitProcess(3, 6);
```
Or
```js
function fruitProcess(apples, oranges) {
//	console.log(apples, oranges);
	const juice = `Juice with ${apples} apples and ${oranges} oranges.`;
	return juice;
}
const appleJuice = fruitProcess(3, 6);
console.log(appleJuice);
```

### Anonymous Function (e.g. function expression)
```js
const calcAge = function (birthYear) {
	return 2022 - birthYear;
}
const age = calcAge(1978);
console.log(age);
```

22.09.2021
### Strict mode
```js
'use strict';
const private = 'Audio';
```

19.09.2021
### Tip calculator
```js
const bill = 300;
const tip = bill <= 500 && bill >= 60 ? bill * 0.15 : bill * 0.2;
console.log(`The bill is ${bill}, the tip is ${tip}, and the total sum is ${bill + tip}`);
```
Challenge 04 from The Complete JavaScript Course 2021: From Zero to Expert!

### Ternary Condition
```js
const age = 23;

age >= 18 ? console.log('Yes, you are allowed to come in.') : console.log('No, you are not allowed to enter.');
```
Other ternary conditional statement
```js
const age = 17;

const drink = age >= 18 ? 'wine' : 'cola';
console.log(drink);
```
Another way of defining it 
```js
let drink2;
if (age >= 18) {
    drink2 = 'wine';
} else {
    drink2 = 'cola';
}
console.log(drink2);
```
Simplified 
```js
const age = 17;

console.log(`I want to drink ${age >= 18 ? 'wine' : 'cola'}`);
```
Tasks from The Complete JavaScript Course 2021: From Zero to Expert!

### Switch Statement
```js
const day = 'Monday';

switch (day) {
    case 'Monday': // day === 'Monday'
        console.log('Day one');
        break;
    case 'Tuesday': 
        console.log('Day two');
        break;
    case 'Wednesday': 
        console.log('Day three');
        break;
    case 'Thursday': 
        console.log('Day four');
        break;    
    case 'Friday': 
        console.log('Day five');
        break;   
    case 'Saturday': 
    case 'Sunday':
        console.log('Weekend');
        break;
    default:
        console.log('Not valid day');
}
```
Compared to an If Statement
```js
const day = 'Monday';

if (day === 'Monday') {
    console.log('Day one');
} else if (day === 'Tuesday') {
    console.log('Day two');
} else if (day === 'Wednesday') {
    console.log('Day three');
} else if (day === 'Thursday') {
    console.log('Day four');
} else if (day === 'Friday') {
    console.log('Day five');
} else if (day === 'Saturday' || day === 'Sunday') {
    console.log('It is weekend');
} else {
    console.log('Not vaild day');
}
```
From The Complete JavaScript Course 2021: From Zero to Expert!

18.09.2021
### Challenge 03 (The Complete JavaScript Course 2021: From Zero to Expert!)
```js
const scoreDolfins = (97 + 112 + 101) / 3;
const scoreKoalas = (109 + 95 + 102) / 3;
console.log(scoreDolfins, scoreKoalas);

if (scoreDolfins > scoreKoalas && scoreDolfins >= 100) {
    console.log('Dolfins win');
} else if (scoreKoalas > scoreDolfins && scoreKoalas >= 100) {
    console.log('Koalas win');
} else if (scoreDolfins === scoreKoalas && scoreDolfins >= 100 && scoreKoalas >= 100) {
    console.log('Both win');
} else {
    console.log('No one wins');
}
```

### Logical operators
```js
const a = true;
const b = true;

if (a && b) {
	console.log('Both are true');
} else {
	console.log('At least of them is false');
}

// Other 
const a = true;
const b = false;

if (a && b) {
	console.log('Both are true');
} else {
	console.log('At least of them is false');
}
```

17.09.2021
### Prompt
```js
prompt("What is your name?");
// or
const yourName = prompt("What is your name?");
console.log(yourName);
```
  
### Equality operator
```js
/*
= - assignment
== - loose equality operator
=== - strick equality operator 
*/
const age = 18;
if (age === 18) console.log('You are grown up!');
```

### 5 falsy values: 0, '', undefined, null, NaN
```js
console.log(Boolean(0));
console.log(Boolean(undefined));
console.log(Boolean('Max'));
console.log(Boolean({}));
console.log(Boolean(''));

// Example
const money = 0;
if (money) {		// The value (money) will be converted into a Boolean
	console.log('Good');
} else {
	console.log('Find a job');
}

// Example 
let height;
if (height) {
	console.log('Height is defined');
} else {
	console.log('Height is undefined');
}
```
  
### Loop multiply by two
```js
for (var i = 2; i < 10000; i *= 2) {
 console.log(i);
}
```
  
16.09.2021
### Convert 'number' to 'string' with String()
```js
const inputNumber = 1991;
const numberToString = String(inputYear);
console.log(numberToString + 3);
```
  
### Convert 'string' to 'number' with Number()
```js
const inputYear = '1991';
const stringToNumber = Number(inputYear);
console.log(stringToNumber + 3);
```
  
### Area of a triangle
```js
function calculateTriangle() {
  let side1 = document.triangleArea.side1.value; 
  let side2 = document.triangleArea.side2.value;  
  let side3 = document.triangleArea.side3.value;  
  
  let sideOne = Number(side1); 
  let sideTwo = Number(side2); 
  let sideThree = Number(side3); 
  
  // Calculation 
 
   let s = (sideOne + sideOne + sideThree) / 2;
   let area =  Math.sqrt(s*((s-sideOne)*(s-sideTwo)*(s-sideThree)));
    document.triangleArea.triangleResult.value = s.toFixed(1);
  }
```
Link - https://codepen.io/achkasoff/pen/jOwaVBr
  
### Condition with comparison
```js
  if(9 > 3){
    console.log('9 is bigger that 3.')
  } else {
    console.log('Strange')
  }
```
  
### Fahrenheit vs. Celsius Converter
```js
  function calculateFc(){
    let fah = document.temperatureConverter.fahrenheit.value; 
    const fahCel = (fah - 32) * 5 / 9;
    document.temperatureConverter.fahrenheitCelsius.value = fahCel.toFixed(2);
  }

  function calculateCf(){
    let cel = document.temperatureConverter.celsius.value; 
    const celFah = cel * 1.8 + 32;
    document.temperatureConverter.celsiusFahrenheit.value = celFah.toFixed(2);
  }
```
Link - https://codepen.io/achkasoff/pen/bGRaEYx
  
### Kilometers vs. Miles Converter
```js
  function calculateKmM(){
    let km = document.distanceConverter.kilometres.value; 
    const conversionFactor = 0.621371;
    let kmM = km * conversionFactor;
    document.distanceConverter.kilometresMiles.value = kmM.toFixed(2);
  }

  function calculateMKm(){
    let m = document.distanceConverter.miles.value; 
    const conversionFactor = 0.621371;
    let mKm = m / conversionFactor; 
    document.distanceConverter.milesKilometres.value = mKm.toFixed(2);
  }
```
Link - https://codepen.io/achkasoff/pen/ZEyvbmm
  
15.09.2021
### What century were you born in?
```js
const birthYear = 2012;
let century;

if (birthYear <= 2000) {
  century = 20;
} else {
  century = 21;
}
console.log(century);
// Other 
function whatCentury() {
  let birthYear = document.centuryForm.birthYear.value;

  if (birthYear <= 2000) {
    document.centuryForm.yourCentury.value = "Your were born in 20th century."
  } else {
    document.centuryForm.yourCentury.value = "Your were born in 21th century."
  }
}
```
Link https://codepen.io/achkasoff/pen/qBjVNqe
  
### if ... else structure
```js
const age = 19;
if(age >= 18){
  console.log("That's ok to learn how to drive");
} else {
  console.log("You're too young. Take your time.");
}

// Other 
const age = 15;
if(age >= 18){
  console.log("That's ok to learn how to drive");
} else {
  const yearsLeft = 18 - age;
  console.log(`You're too young. Wait for another ${yearsLeft} years.`);
}
```
  
### Concatenation / Template literals
```js
const firstName = 'Maxim';
const job = 'teacher';
const subject = "Business English";
const birthYear = 1978;
const thisYear = 2021;

const maxim = "I'm " + firstName + ", a " + (thisYear - birthYear) + "-year-old " + job + " of " + subject + "!";
console.log(maxim);

// Template literals
const maximNew = `I'm ${firstName}, a ${thisYear - birthYear}-year-old ${job} of ${subject}!`;
console.log(maximNew);
```
  
### Challenge 01 (The Complete JavaScript Course 2021 From Zero to Expert!)
```js
// Data 1: Marks weights 78 kg and is 1.69 m tall. John weights 92 kg and is 1.95m tall.
let markMass = 78;
let markHeight = 1.69;
let johnMass = 92;
let johnHeight = 1.95;

let bmiMark = markMass / markHeight ** 2;
let bmiJohn = johnMass / johnHeight ** 2;
let markHigherBMI = bmiMark > bmiJohn;
console.log(bmiMark, bmiJohn, markHigherBMI); 

// Data 2: Marks weights 95 kg and is 1.88 m tall. John weights 85 kg and is 1.76m tall.
let markMass = 95;
let markHeight = 1.88;
let johnMass = 85;
let johnHeight = 1.76;

let bmiMark = markMass / markHeight ** 2;
let bmiJohn = johnMass / johnHeight ** 2;
let markHigherBMI = bmiMark > bmiJohn;
console.log(bmiMark, bmiJohn, markHigherBMI); 
```
  
### BMI calculation
```js
function calculateBmi() {
  // Get numbers from input
  let weight = document.BMIform.weight.value;
  let height = document.BMIform.height.value;

  // BMI calculation
  if(weight > 0 && height > 0){	
  let totalBmi = weight/(height*height);
  // Return result in HTML
  document.BMIform.bmiResult.value = totalBmi.toFixed(2);

  // Condition
  if(totalBmi < 18.5){
  document.BMIform.means.value = "Try eating more."
  }
    
  if(totalBmi > 18.5 && totalBmi < 25){
  document.BMIform.means.value = "You are ok."
  }
    
  if(totalBmi > 25 &&  totalBmi <30){
  document.techBMI.means.value = "You are a bit overweight."
  }
  
  if(totalBmi > 30){
  document.BMIform.means.value = "Sorry, but you've got to do something."
  }
 } else {
   alert("Data you've entered might be incorrect. Please check and try again.")
  }
}
```
  
14.09.2021
### Roll Dice
```js
let response;
let a = randomNum(5);
let b = randomNum(6);

function rollDice(num1, num2){
if(num1 > num2){
  response = "Number 1 wins";
  }else if(num1 == num2){
  response = "Draw";
  }else{
  response = "Number 2 wins";
}
return response;
}
function randomNum(val){
	return Math.floor(Math.random() * val) + 1;
}
let message = rollDice(a, b);
console.log(a + " vs " + b + " " + message);
```
  
### Assignment oprators
```js
let x = 10 + 5;
x += 10;
x *= 4;
x++;
x--;
console.log(x);
```
  
### Math.ceil() To round a number up
```js
const number = 923.2238;
console.log(Math.ceil(number));
```

### Math.pow() - Base, Exponent 
```js
console.log(Math.pow(7, 2));
// Returns 49
```

### Interpolation 
```js
const nameInput = 'Maxim';
console.log(`Do you want to eat, ${nameInput}?`);
```

### Concatenation
```js
let info = "We couldn't verify you mother's maiden name.";
let intro = 'Here is important information about your account security.';

let firstName = 'Joffrey';
let greeting = 'Hello, ';

let firstLine = greeting + firstName + "!" + "\n";
let bodyLetter = intro + "\n" + info;

console.log(firstLine + bodyLetter);
```

### Currency converter
```js
let eurosCount = 100;
let dollarCount = eurosCount * 1.25;
let rublesCount = dollarCount * 60;
console.log("The price is " + rublesCount + " rubles");
```
      
12.09.2021
### Twice as old
```js
function twiceAsOld(dadYearsOld, sonYearsOld) {
	return Math.abs(dadYearsOld - (2 * sonYearsOld));
	}
console.log(twiceAsOld(64, 32));
```

### Multiplication
```js
function multiplication(a, b) {
  return a * b;
}
let result = multiplication(3, 5);
console.log(result);

```

### Ternary Operator 
```js
let price = 10;
let day = "Sunday";

day === "Sunday" ? price - 1 : price + 1;
```

### String Interpolation 
```js
let age = 43;
let message = `Max is ${age} years old.`;
console.log(message);
```

11.09.2021
### Condition
```js
let boolOne = 5 > 3;
let boolTwo = 5 < 3;

if(boolOne){
  console.log("That's right");
  }else{
  console.log("That's wrong");
}
```

### Roll Dice 
```js
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

### Condition (Message)
```js
let message = (5 == 5) ? 'TRUE' : 'FALSE';
console.log(message);
```

### Randon Number (from 0 to 5)

```js
Math.floor(Math.random() * 5);
```
  

### Randon Number (from 1 to 5)

```js
Math.floor(Math.random() * 5) + 1;
```

### Code (Unresolved)
```js
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
  
10.09.2021
### MakeUpperCase
```js
function makeUpperCase(str) {
  let string = str.toUpperCase()
  return string
}
```

### Grasshopper - Summation
```js
var summation = function (num) {
    let totalSum = 0
    for(let i = 0; i <= num; i++) {
        totalSum = i + totalSum
    }
    return totalSum
}
```

09.09.2021
### if ... else clause 
```js
const size = 10;
if (size > 100) {
  console.log('Big');
} else if (size > 20) {
  console.log('Middle');
} else if (size > 4) {
  console.log('Small');
} else { 
  console.log('Tiny');
}
```
