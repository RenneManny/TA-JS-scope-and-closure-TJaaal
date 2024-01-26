Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(useranme); Reference error username is not defined.
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(useranme);Reference error username is not defined.
```
In the above code we are looking for a variable named `username`. The usernme is defined inside the block scope hence we cannot access the variable outside the scope.

The above cde will throw an error `Reference error username is not defined`.
3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(useranme); Reference error username is not defined.
```
In the above code we are assigning `username="Arya" ` in block scope .Therefore we cannot access it outside the scope.

The above code will throw an error naming:`Reference error username is not defined. `
4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(useranme); // Arya
```
In the above code we are asigning a `username =Arya` using var keyword. variables defined using var keyword have global and functional scope . In this case it username is global scoped. Hence we can access the username outside the scope.

The output of the above code will be:-Arya
5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(useranme); // syntaxError username has already been declared
```
In the above code,on first line we are asigning a `username =Arya` using let keyword. variables defined using let  keyword can only be declared once. In this case we are redeclaring it inside scope using var which will result in error.

Output of the above code will be :- `syntaxError username has already been declared '.

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(useranme); // `syntaxError username has already been declared '
```
In the above code,on first line we are asigning a `username =John ` using let keyword. variables defined using let  keyword can only be declared once and can be reassigned .But, In this case we are redeclaring it inside scope using let keyword again  which will result in error.

Output of the above code will be :- `syntaxError username has already been declared '.
7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(useranme); // `syntaxError username has already been declared '.
```
In the above code,on first line we are asigning a `username =John ` using let keyword. variables defined using let  keyword can only be declared once and can be reassigned .But, In this case we are redeclaring it inside function  using let keyword again  which will result in error.

Output of the above code will be :- `syntaxError username has already been declared '.
8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
}
console.log(i, 'Second'); // output
```

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First'); // output
}
console.log(i, 'Second'); // output
```
