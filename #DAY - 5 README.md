# DAY 5: JavaScript Functions

## Table of Contents

1. [Activity 1: Funtion Declaration](#activity-1-function-declaration)
   - Task 1: Function to check if a number is even or odd
   - Task 2: Function to calculate the square of a number
2. [Activity 2: Function Expression](#activity-2-function-expression)
   - Task 3: Function Expression to find the maximum of two numbers
   - Task 4: Function Expression to concatenate two strings
3. [Activity 3: Arrow Functions(#activity-3-arrow-functions)
   - Task 5: Arrow function to calculate the sum of two numbers
   - Task 6: Arrow function to check if the string is contain a specific characters
4. [Activity 4: Function Parameters and Default Values](#activity-4-function-parameters-and-default-values)
   - Task 7: Function that take two parameters and return their products and default value for the second parameters
   - Task 8: Function that takes person name and age and return a greeting message and takes default value for the age
5. [Activity 5: Higher-Order Functions](#activity-5-higher-order-functions)
   - Task 9: A higher order function that takes a function and a number, and call the function that many times
   - Tase 10: A higher order function that takes two functions and a value, applies the first function to the value, and then apply the second function to the result
6. [Feature Request](#feature-request)
   - 1. Even or Odd Function Script
   - 2. Square Calculation Function Script
   - 3. Concatenation Function Script
   - 4. Sum Caluculation Arrow Function Script
   - 5. Higher-Order Function Script
7. [Achievements](#achievements)

## Activity 1: Function Declaration

**Task 1:** Write a function to check if a number is even or odd and log the result to the console.

```javascript
function evenOrOdd(n) {
  if(n%2 == 0) {
    console.log(`${n} is even number`);
  }
  else {
    console.log(`${n} is odd number`);
  }
}
evenOrOdd(20); // 20 is even number
evenOrOdd(15); // 15 is odd number
```

**Task 2:** Write a function to calculate the square of a number and result the console.

```javascript
function findSquare(n) {
  let ans = n*n;
  return ans;
}
let ans = findSquare(10);
console.log("square is: ", ans); // square is : 100
```

## Activity 2: Function Expression

**Task 3:** Write a Function Expression to find the maximum of two numbers and log the result to the console.

```javascript
let findMax = function (n1,n2) {
  let ans = n1 > n2 ? n1 : n2;
  console.log(`Maximum of ${n1} and ${n2} is ${ans}`);
}
findMax(25,50); // Maximum of 25 and 50 is 50
```

**Task 4:** Write a Function Expression to concatenate two strings and return the result.

```javascript
let concatenateString = function (str1, str2) {
  return str1 + str2;
}
console.log(concatenateString("Hello", " Arun")); // Hello Arun
```

## Activity 3: Arrow Functions

**Task 5:** Write an arrow function to calculate the sum of two numbers and return the result.

```javascript
let sum = (n1,n2) => n1 + n2 ;
console.log(sum(25,35)); // 60
```

**Task 6:** Write an arrow function to check if a string contains a specific characters and return a boolean value.

```javascript
let isPresent = (str,ch) => str.includes(ch);
console.log(isPresent("Arun",'r')); // true
console.log(isPresent("Code Help", 'y')); // false
```

## Activity 4: Function Parameters and Default Values

**Task 7:** Write a function that takes two parameters and return their product. Provide a default value for the second parameter.

```javascript
function findProduct(n1, n2 = 10) {
    return n1 * n2;
}
console.log(findProduct(20)); //output : 200
console.log(findProduct(10,13)); //output : 130
```

**Task 8:** Write a function that takes a person's name and age and returns a greeting message. Provide default value for the age.

```javascript
function greetings(name,age = 20) {
    console.log(`Hello ${name}, You are ${age} Years old.`);
}
greetings("Arun"); //Output: Hello Arun, You are 20 Years old.
```

## Activity 5: Higher-Order Functions

**Task 9:** Write a higher-order function that takes a function and a number, and calls the function that many times.

```javascript
function repeatFunction(fn,n) {
    for(let i=0;i<n;i++) {
        fn();
    }
}
repeatFunction( ()=> console.log("Arun"),4);
/*Expected Output: 
Arun
Arun
Arun
Arun */
```

**Task 10:** Write a higher-order function that takes two functions and a value, applies the first function to the value, and then applies the second function to the result.

```javascript
function find(f1,f2,val) {
    return f2(f1(val));
}

let add = (n) => n+5;
let square = (n) => n*n;
console.log(find(add,square,10)); // Output : 225
```

## Feature Request:

1. Write a script that includes a function to check if a number is even or odd and logs the result.

2. Create a script that includes a function to calculate the square of a number and returns the result.

3. Write a script that includes a function expression to concatenate two strings and returns the result.

4. Create a script that includes an arrow function to calculate the sum of two numbers and returns the result.

5. Write a script that includes a higher-order function to apply a given function multiple times.

## Achievements:

By the end of these activities, students will:

- Understand and define functions using function declarations, expressions, and arrow functions.

- Use function parameters and default values effectively.

- Create and utilize higher-order functions.

- Apply functions to solve common problems and perform calculations.

- Enhance code reusability and organization using functions.
