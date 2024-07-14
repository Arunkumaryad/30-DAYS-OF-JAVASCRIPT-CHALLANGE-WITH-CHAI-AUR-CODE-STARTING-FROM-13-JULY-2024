# DAY 2: JavaScript Operators

## Table of Contents

1. [Activity 1: Arithmetic Operations](#activity-1-arithmetic-operations)
   - Task 1: Addition
   - Task 2: Subtraction
   - Task 3: Multiplication
   - Task 4: Division
   - Task 5: Remainder
2. [Activity 2: Assignment Operators](#activity-2-assignment-operators)
   - Task 6: `+=` Operator
   - Task 7: `-=` Operator
3. [Activity 3: Comparison Operators](#activity-3-comparison-operators)
   - Task 8: `>` and `<` Operators
   - Task 9: `>=` and `<=` Operators
   - Task 10: `==` and `===` Operators
4. [Activity 4: Logical Operators](#activity-4-logical-operators)
   - Task 11: `&&` Operator
   - Task 12: `||` Operator
   - Task 13: `!` Operator
5. [Activity 5: Ternary Operator](#activity-5-ternary-operator)
   - Task 14: Ternary Operator
6. [Feature Request](#feature-request)
   - 1. Arithmetic Operations Script
   - 2. Comparison and Logical Operators Script
   - 3. Ternary Operator Script
7. [Achievements](#achievements)

## Activity 1: Arithmetic Operations

**Task 1:** Write a Program to add two numbers and log the result to the console.

```javascript
let a = 5;
let b = 3;
console.log("Sum:", a+b); // Sum: 8
```

**Task 2:** Write a Program to subtract two numbers and log the result to the console.

```javascript
let a = 50;
let b = 40;
console.log("Sub is : ", a-b); // Sub is : 10
```

**Task 3:** Write a Program to multiply two numbers and log the result to the console.

```javascript
let a = 10;
let b = 40;
console.log("Prod is : ", a*b); // Prod is : 400
```

**Task 4:** Write a Program to divide two numbers and log the result to the console.

```javascript
let a = 120;
let b = 40;
console.log("Div is : ", a/b); // Div is : 3
```

**Task 5:** Write a Program to find the remainder when one number is devided by another and log the result to the console.

```javascript
let a = 50;
let b = 13;
console.log("Rem is : ", a%b); // Rem is : 11
```

## Activity 2: Assignment Operators

**Task 6:** Use the `+=` Operators to add a number to the variable and log the result to the console.

```javascript
let a = 50;
a += 10;
console.log("a is : ", a); // a is : 60
```

**Task 7:** Use the `-=` Operators to subtract a number to the variable and log the result to the console.

```javascript
let a = 50;
a -= 10;
console.log("a is : ", a); // a is : 40
```

## Activity 3: Comparison Operators

**Task 8:** Write a Program to compare two number using `>` and `<` and log the result to the console.

```javascript
let a = 20;
let b = 10;
console.log("a > b is: ", a > b); // a > b is: true
console.log("a < b is: ", a < b); // a < b is: false
```

**Task 9:** Write a Program to compare two number using `>=` and `<=` and log the result to the console.

```javascript
let a = 20;
let b = 10;
console.log("a >= b is: ", a > b); // a >= b is: true
console.log("a <= b is: ", a < b); // a <= b is: false
```

**Task 10:** Write a Program to compare two number using `==` and `===` and log the result to the console.

```javascript
let a = 10;
let b = '10';
console.log("a == b is: ", a == b); // a == b is: true
console.log("a === b is: ", a === b); // a === b is: false
```

## Activity 4: Logical Operators

**Task 11:** Write a Program that uses the `&&` operator to combine two conditions and log the result to the console.

```javascript
let a = false;
let b = true;
console.log("a && b is: ", a && b); // a && b is: false
```

**Task 12:** Write a Program that uses the `||` operator to combine two conditions and log the result to the console.

```javascript
let a = false;
let b = true;
console.log("a || b is: ", a || b); // a || b is: true
```

**Task 13:** Write a Program that uses the `!` operator to negate a conditions and log the result to the console.

```javascript
let a = false;
console.log("!a is: ", !a); // !a is: true
```

## Activity 5: Ternary Operators

**Task 14:** Write a Program that uses the ternary operator to check if a number is negative or positive and log the result to the console.

```javascript
let a = 10;
let ans = (a > 0) ? "Postive" : "Negative";
console.log("Ans is:", ans); // Ans is: Positive
```

## Feature Request:

### Arithmetic Operaions Script:

Write a Script that performs basic arithmetic operations **(addition, subtraction, multiplication, devision, remainder)** on two numbers and logs the results.

```javascript
let a = 20;
let b = 12;

//Addition
let sum = a + b;
console.log("Sum:", sum); // Sum: 32

// Subtraction
let diff = a - b; 
console.log("Diff:", diff); // Diff : 8

//Multiplication
let prod = a * b;
console.log("Prod:", prod); // Prod: 240

//Division
let div = a / b;
console.log("Div:", div); // Div: 1

//Remainder
let ans = a % b;
console.log("ans:", ans); //ans: 8
```

### Comparison and Logical Operators Script:

Create a Script that compares two numbers using different comparison operators and combines conditions using logical oprators, logging the results.

```javascript
let a = 25;
let b = 30;

//comparision operators
console.log("a > b is:", a > b); // false
console.log("a < b is:", a < b); // true
console.log("a >= b is:", a >= b); // false
console.log("a <= b is:", a <= b); // true
console.log("a == b is:", a == b); // false
console.log("a === b is:", a === b); // false

//Logical Operators.
let cond1 = a < b; 
let cond2 = a > 0; 
console.log(cond1); // true
console.log(cond2); // true

//Logical AND (&&)
console.log("cond1 && cond2 is:", cond1 && cond2); // true 

//Logical OR (||)
console.log("cond1 || cond2 is:", cond1 || cond2); // true

//Logical NOT (!)
console.log("!cond1 is:", !cond1); // false
```

### Ternary Operator Script:

Write a Script that uses the ternary operator to determine if a number is positive or negative and logs the result.

```javascript
let num = -15;
let ans = (num > 0) ? "Positive" : "Negative";
console.log(ans); // Negative
```

## Achievements:

By the end of these activities, students will:

- Understand and use arithmetic operators to perform basic calculations.
- Use assignment operators to modify variable values.
- Compare values using comparison operators.
- Combine conditions using logical operators.
- Use the ternary operator for concise conditional expressions.
