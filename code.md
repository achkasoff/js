# JS Code

11.09.2021
### Condition
let boolOne = 5 > 3;
let boolTwo = 5 < 3;

if(boolOne){
console.log("That's right");
}else{
console.log("That's wrong");
}

--------
### Roll Dice 
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

-------

