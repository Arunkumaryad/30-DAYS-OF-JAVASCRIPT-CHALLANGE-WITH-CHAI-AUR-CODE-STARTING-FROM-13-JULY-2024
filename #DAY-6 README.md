
# DAY 6: JavaScript Arrays

## Table of Contents

1. [Activity 1: Array Creation and Access](#activity-1-array-creation-and-access)
   - Task 1: Create an array of numbers from 1 to 5 and log the array to the console.
   - Task 2: Access the first and last elements of the array and log them to the console.
2. [Activity 2: Array Methods(Basic)](#activity-2-array-methods-basic)
   - Task 3: Use the `push` method to add a new number to the end of the array and log the updated array.
   - Task 4: Use the `pop` method to remove the last element from the array and log the updated array.
   - Task 5: Use the `shift` method to remove the first element from the array and log the updated array.
   - Task 6: Use the `unshift` method to add a new number to the beginning of the array and log the updated array.
3. [Activity 3: Array Methods (Intermediate)](#activity-3-array-methods-intermediate)
   - Task 7: Use the `map` method to create a new array where each number is doubled and log the new array.
   - Task 8: Use the `filter` method to create a new array with only even numbers and log the new array.
   - Task 9: Use the `reduce` method to calculate the sum of all numbers in the array and log the result.
4. [Activity 4: Array Iteration](#activity-4-array-iteration)
   - Task 10: Use a `for` loop to iterate over the array and log each element to the console.
   - Task 11: Use the `forEach` method to iterate over the array and log each element to the console.
5. [Activity 5: Multi-dimensional Arrays](#activity-5-multi-dimensional-arrays)
   - Task 12: Create a two-dimensional array (matrix) and log the entire array to the console.
   - Tase 13: Access and log a specific element from the two-dimensional array.
6. [Feature Request](#feature-request)
   - 1. Array Manipulation Script
   - 2. Array Transformation Script
   - 3. Array Iteration Script
   - 4. Two-dimensional Array Script
7. [Achievements](#achievements)

## Activity 1: Array Creation and Access

**Task 1:** Create an array of numbers from 1 to 5 and log the array to the console.

```javascript
let arr = [1,2,3,4,5];
console.log(arr); //Output : [ 1, 2, 3, 4, 5 ]
```

**Task 2:** Access the first and last elements of the array and log them to the console.

```javascript
let arr = [1,2,3,4,5,6];
console.log(arr[0]);  //Output : 1
console.log(arr.length-1); //Output : 5
```

## Activity 2: Array Methods (Basic)

**Task 3:** Use the push method to add a new number to the end of the array and log the updated array.

```javascript
let arr = [1,2,3,4,5];
arr.push(10);
console.log(arr); //Output : [ 1, 2, 3, 4, 5, 10 ]
```

**Task 4:** Use the pop method to remove the last element from the array and log the updated array.

```javascript
let arr = [2,4,6,8,10];
arr.pop();
console.log(arr); //Output : [ 2, 4, 6, 8 ]
```

**Task 5:** Use the shift method to remove the first element from the array and log the updated array.

```javascript
let arr = [1,2,3,4,5];
arr.shift();
console.log(arr); //Output : [ 2, 3, 4, 5 ]
```

**Task 6:** Use the unshift method to add a new number to the beginning of the array and log the updated array.

```javascript
let arr = [2,4,6,8];
arr.unshift(10);
console.log(arr); //Output : [ 10, 2, 4, 6, 8 ]
```

## Activity 3: Array Methods (Intermediate)

**Task 7:** Use the map method to create a new array where each number is doubled and log the new array.

```javascript
let arr = [1,2,3,4,5];
let newArr = arr.map((num) => num*2);
console.log(newArr); //Output : [ 2, 4, 6, 8, 10 ]
```

**Task 8:** Write an arrow function to check if a string contains a specific characters and return a boolean value.

```javascript
let arr = [1,2,4,6,8];
let newArr = arr.filter((num) => num%2 == 0);
console.log(newArr); // output : [ 2, 4, 6, 8 ]
```

**Task 9:** Use the reduce method to calculate the sum of all numbers in the array and log the result.

```javascript
let arr = [1,2,3,4,5];
let sum = arr.reduce((accumulator,currValue) => accumulator + currValue)
console.log(sum); // Output : 15
```

## Activity 4: Array Iteration

**Task 10:** Use a for loop to iterate over the array and log each element to the console.

```javascript
let arr = [1,2,3,4,5];
let n = arr.length;
for(let i=0;i<n;i++) {
    console.log(arr[i]);
}
/* Expected Output : 
1
2
3
4
5 */
```

**Task 11:** Use the forEach method to iterate over the array and log each element to the console.

```javascript
let arr = [1,2,3,4,5];
arr.forEach((ele) => console.log(ele));
/* Expected Output : 
1
2
3
4
5 */
```

## Activity 5: Multi-dimensional Arrays

**Task 12:** Create a two-dimensional array (matrix) and log the entire array to the console.

```javascript
let arr = [
     [1,2,3,4],
     [5,6,7,8],
     [9,10,11,12]
    ];
console.log(arr);
/* Expected Outpuut : 
[ [ 1, 2, 3, 4 ], [ 5, 6, 7, 8 ], [ 9, 10, 11, 12 ] ] */
```

**Task 13:** Access and log a specific element from the two-dimensional array.

```javascript
let matrix = [
    [1,2,3],
    [4,5,6],
    [7,8,9]
];
let element = matrix[2][2];
console.log(element); //Output : 9
```

## Feature Request:

1. Write a script that demonstrates the creation of an array, adding and removing elements using push, pop, shift, and unshift methods.

2. Create a script that uses map, filter, and reduce methods to transform and aggregate array data.

3. Write a script that iterates over an array using both for loop and forEach method and logs each element.

4. Create a script that demonstrates the creation and manipulation of a two-dimensional array.


## Achievements:

By the end of these activities, students will:

- Create and manipulate arrays using various methods.
- Transform and aggregate array data using map, filter, and reduce.
- Iterate over arrays using loops and iteration methods.
- Understand and work with multi-dimensional arrays.
