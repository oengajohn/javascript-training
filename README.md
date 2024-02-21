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

```

