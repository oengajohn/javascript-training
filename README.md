# Javascript Training

## Walkthrough

```javascript
function add (a, b){
return a +b;
}
console.log(add(5,-12)); 

var clickMe = document.getElementById("clickMe");

clickMe.addEventListener('click',(event) => {
  alert("You clicked me");
}); 
clickMe.addEventListener("click", function(event){
     fetch("https://jsonplaceholder.typicode.com/todos")
       .then((response) => response.json())
       .then((todos) => {
            todos.forEach(todo => {
               var todoElement =  `<p>${todo.title}</p>`;
             console.log(todoElement);
            });
       });
});
```
## Variables
```javascript
let result = 20; // var
function sum(a,b){
  result = a + b;
  return result;
}
console.log(result);
console.log(sum(15,12));
console.log(result);

let message = "Hello World";
console.log(message);
message = "Test";
console.log(message);

// variable which don't change
const PI = 3.142;

function area(radius){
  return PI *  radius * radius;
}
console.log(area(5));

console.log(PI);

const add = (a,b) => a+b;

console.log(add(5,18));

let age=20;

console.log("My Age is " + age);

let studentName="Mackrine"

console.dir(studentName);
console.dir(studentName.split(""));
console.dir(studentName.toUpperCase(""));
console.dir(studentName.toLowerCase(""));
console.dir(studentName.includes("ack"));
```
## Data types

```javascript
let stringVariable = "hello";
console.log(typeof stringVariable);

let age = 20.25;
console.log(typeof age);

var testUndefined ;
console.log(typeof testUndefined);

var testNull = null;
console.log(typeof testNull);

var  test=false
console.log(typeof test);

let fruits = [ "Orange", "Banana", "Mango", "Madafu"]

var array = new Array(fruits);

console.log(typeof fruits);
console.log(typeof array);
console.log(typeof 10n);

var student = {

}
console.log(typeof student);

```

## Interaction with alert, confirm, prompt
```javascript
// interaction with alert, confirm, prompt

// alert("Hello, your door bell is not working")
/* let isBoss = confirm("Is Musili in class?")
console.log(isBoss); */

let ageString = prompt("What is your age?")
console.log(typeof ageString);
console.log( ageString);



```

## Data Conversions

```javascript
let ageString = prompt("What is your age?")
console.log(typeof ageString);
//number
let age = Number(ageString);
console.log(typeof age)
console.log( age)

// let isBoss = confirm("Is your boss?");
// console.log(typeof isBoss);

let myAgeIs = `My Age is ${age}`;

let isAgeSet = Boolean(myAgeIs);
console.log(myAgeIs);

console.log(typeof isAgeSet) // number
console.log( isAgeSet)

let myAgeIs2 = '';
console.log(myAgeIs2);
let isAgeSet2 = Boolean(myAgeIs2); 
console.log(typeof isAgeSet2);
console.log(isAgeSet2); // false

alert("6" / "2") // 3

let ageTwoSTring = String(age)
console.log(typeof ageTwoSTring) //string
console.log( ageTwoSTring)

let test= null;
let test2= undefined;

let numberOne = Number(test); // 0
console.log(typeof numberOne);
console.log(numberOne);


let numberTwo = Number(test2); //undefined
console.log(typeof numberTwo);
console.log(numberTwo); //NaN
```


