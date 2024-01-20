1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here

// function expression
let percentage=function(marks,total){
  return (marks*100)/total;
}
// arrow function
let percentage=(marks,total)=>{
  return (marks*100)/total;
}
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer
// function declaration
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
// function expression/Annonymous function
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
// function expression/Annonymous function
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
// arrow function
```

```js
let percentage = (marks, total) => (marks * 100) / total;
// arrow function
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.
<!-- As we know function is an object. And also we can assign function to a variable . Therefore we can asign a function to a variable and can conduct various operations on it. -->
```js
let fullName=function(name,surname){
  return `${name} ${surname}`;

}
```
4. Why is a function call an expression in JavaScript?
<!-- A function call is an expression because it produces a value. When function is invoked, it executes its code and returns a result. -->
5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // Valid because it will calculate the value and assign to five which is a variable.
five = add; // Invalid becuase here we are not using () after add. This mean it is not functio call but a function reference.
five = five(10, 11); // invalid because five is a variable not a function
five = function () {
  return 'Hello';
}; // Valid because it function expression or annoymous function 
```

6. What is the difference between function definition and function call? Explain with an example.

<!-- Function Definition :->Function definition is the process of defining what function will do when it will be executed.But the function call means that you have called a function.Function is defined by using function keyword where as function call is done by placing () before function name . 
eg -->
```js
// function declaration 
function greet(name){
  return `Good morning ${name}`;
}
// function call
greet("Akhil");
```

7. What is the similarities between function definition and function call?
<!-- The first one is, it is the whole process of performing one or more task -->
<!-- We use () whether there is some parameter or not . -->
8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // invalid The code is invalid because hello is a function not an object .
```

9. What is higher order function explain with an example.
<!-- A higher-order function in JavaScript is a function that takes one or more functions as arguments or returns a function as its result -->
10. Explain what is callback function. Why you can pass a function inside a function?
<!-- A callback function in JavaScript is a function that is passed as an argument to another function  -->
