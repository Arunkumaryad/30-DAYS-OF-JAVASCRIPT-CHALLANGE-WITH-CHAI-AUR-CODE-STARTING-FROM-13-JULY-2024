
# DAY 8: JavaScript ES6 + Features

## Table of Contents

1. [Activity 1: Template Literals](#activity-1-template-literals)
   - Task 1: Use template literal to create a string that includes variables for a person's name and age, and log the string to the console.
   - Task 2: Create a multi-line string using template literals and log it to the console.
2. [Activity 2: Destructuring](#activity-2-destructuring)
   - Task 3: Use array Destructuring to extract the first and second elements from an array of numbers and log them to the console.
   - Task 4: Use object destructuring to extract the title and author from a book object and log them to the console.
3. [Activity 3: Spread and Rest Operators](#activity-3-spread-and-rest-operators)
   - Task 5: Use the spread operator to create a new array that includes all elements of an exsiting array plus additional elements, and log the new array to the console.
   - Task 6: Use the rest operator in a function to accept an arbitary number of arguments, sum them, and return the result.
4. [Activity 4: Default Parameters](#activity-4-default-parameters)
   - Task 7: Write a function that takes two parameters and returns their product, with the second parameter having a default value of 1. Log the result of calling this 
             function with without the second parameter.
5. [Activity 5: Enhanced Object Literals](#activity-5-multi-dimensional-arrays)
   - Task 8: Use enhanced object literals to create an object with method and properties, and log the object to the console.
   - Tase 9: Create an Object with computed property names based on variables and log the object to the console.
6. [Feature Request](#feature-request)
   - 1. Template Literals Script
   - 2. Destructuring Script
   - 3. Spread and Rest Operator Script
   - 4. Default Parameters Script
   - 5. Enhanced Object Literals Script
7. [Achievements](#achievements)

## Activity 1: Template Literals

**Task 1:** Use template literal to create a string that includes variables for a person's name and age, and log the string to the console.

```javascript
const name = "John Due";
const age = 25;
console.log(`My name is ${name} and I am ${age} years old.`)
//Output: My name is John Due and I am 25 years old.
```

**Task 2:** Create a multi-line string using template literals and log it to the console.

```javascript
const str = `My name is John Due.
I am a B.Tech Passout Student.
Now I am exploring DSA`;
console.log(str);
/* Output: My name is John Due.
I am a B.Tech Passout Student.
Now I am exploring DSA */
```

## Activity 2: Destructuring

**Task 3:** Use array Destructuring to extract the first and second elements from an array of numbers and log them to the console.

```javascript
let arr = [10,20,30,40,50];
let [first,second] = arr;
console.log(`First element is: ${first} and second element is: ${second}`);
//Output: First element is: 10 and second element is: 20
```

**Task 4:** Use object destructuring to extract the title and author from a book object and log them to the console.

```javascript
const book = {
    title: "JavaScript with masti",
    author: "HC",
    year: 2024
}
const {title, author} = book;
console.log(`Title is: ${title} and Author is: ${author}`);
//Output: Title is: JavaScript with masti and Author is: HC
```


## Activity 3: Spread and Rest Operators.

**Task 5:** Use the spread operator to create a new array that includes all elements of an exsiting array plus additional elements, and log the new array to the console.

```javascript
const arr = [10,20,30];
const newArr = [...arr,50,60,80];
console.log(newArr); //Output : [ 10, 20, 30, 50, 60, 80 ]
```

**Task 6:** WUse the rest operator in a function to accept an arbitary number of arguments, sum them, and return the result.

```javascript
function sum(...num) {
    return num.reduce((ans,n) => ans+n,0);
}
console.log(sum(1,2,3,4,5)); // Output: 15
```


## Activity 4: Default Parameters

**Task 7:** Write a function that takes two parameters and returns their product, with the second parameter having a default value of 1. Log the result of calling this 
             function with without the second parameter

```javascript
function multiplication(n1,n2=1) {
    return n1*n2;
}
console.log(multiplication(5)); //Output: 5
console.log(multiplication(10,25)); //Output: 250
```


## Activity 5: Enhanced Object Literals

**Task 8:** Use enhanced object literals to create an object with method and properties, and log the object to the console.

```javascript
const name = "Arun Kumar";
const age = 24;
const person = {
    name,
    age,
    greeting() {
        console.log(`My name is ${this.name} and I am ${this.age} Years old.`);
    }
};
console.log(person); 
person.greeting();
/* output: 
{ name: 'Arun Kumar', age: 24, greeting: [Function: greeting] }
My name is Arun Kumar and I am 24 Years old. */
```

**Task 9:** Create an Object with computed property names based on variables and log the object to the console.

```javascript
const key = "favourite youtuber";
const value = "Elvish Yadav";
const Best = {
    [key] : value
}
console.log(Best); 
//Output: { 'favourite youtuber': 'Elvish Yadav' }
```

## Feature Request:

1. Write a script that demonstrates the use of template literals to create and log strings with embedded variables and multi-line strings.

2. Create a script that uses array and object destructuring to extract values and log them.

3. Write a script that demonstrates the use of the spread operator to combine arrays and the rest operator to handle multiple function arguments.

4. Create a script that defines a function with default parameters and logs the results of calling it with different arguments.
5. Write a script that uses enhanced object literals to create and log an object with methods and computed property names.


## Achievements:

By the end of these activities, students will:

- Understand and use template literals for string interpolation and multi-line strings.
- Utilize array and object destructuring to extract values from arrays and objects.
- Apply the spread and rest operators for various use cases including function arguments and array manipulation.
- Implement default parameters in functions.
- Create and manage objects with enhanced object literals for cleaner and more concise code.
