1. Create a function by your choice that accepts a callback function.
```js

function performOperation(a, b, operationCallback) {
  
    const result = operationCallback(a, b);

    console.log(`Result: ${result}`);
}

function add(a, b) {
    return a + b;
}

function subtract(a, b) {
    return a - b;
}

performOperation(5, 3, add); 

performOperation(10, 4, subtract); 


```
2. Create a function by you choice that returns a function reference.

3. Create a higher order function called `map` that takes two inputs:
   - An array of numbers/string/boolean etc
   - A 'callback' function - a function that is applied to each element of the array (inside of the function 'map')

Have `map` return a new array filled with values that are the result of the 'callback' function on each element of the input array.

```js
function map(array, callback) {
    const resultArray = [];

    for (let i = 0; i < array.length; i++) {
        
        resultArray.push(callback(array[i]));;
    }

    return resultArray;
}

// Test Your Code
function multiplyByTwo(n) {
    return n * 2;
}

const mappedArray = map([1, 2, 3, 4, 5], multiplyByTwo);
console.log(mappedArray); // Output: [2, 4, 6, 8, 10]

console.log(multiplyByTwo(1)); // Output: 2
console.log(multiplyByTwo(2)); // Output: 4

```

4. Create a higher-order function called `forEach` taht takes an array and a callback, and runs the callback on each element of the array. `forEach` does not return anything.

```js
function forEach(array, callback) {
    for (let i = 0; i < array.length; i++) {
        callback(array[i]);
    }
}

// Test Your Code
let alphabet = '';
let letters = ['a', 'b', 'c', 'd'];
forEach(letters, function(char) {
    alphabet += char;
});
console.log(alphabet);

// Test Your Code
let alphabet = '';
let letters = ['a', 'b', 'c', 'd'];
forEach(letters, function (char) {
  alphabet += char;
});
console.log(alphabet); //prints 'abcd'
```

5. Create higher-order function called `filter` takes an array and a callback, and runs the callback on each element of the array if the return value of callback is `truthy` store in new array return the new array.

```js
// Test Your Code

function filter(array, callback) {
    const resultArray = [];

    for (let i = 0; i < array.length; i++) {
        if (callback(array[i])) {
            resultArray.push(array[i]);
        }
    }

    return resultArray;
}

// Test Your Code
var numbers = [1, 3, 5, 4, 7, 89, 234, 20];

let even = filter(numbers, function(n) {
    return n % 2 === 0;
});
console.log(even); // Output: [4, 234, 20]

let odd = filter(numbers, function(n) {
    return n % 2 !== 0;
});
console.log(odd); // Output: [1, 3, 5, 7, 89]

```
