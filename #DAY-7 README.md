
# DAY 7: JavaScript Objects

## Table of Contents

1. [Activity 1: Object Creation and Access](#activity-1-object-creation-and-access)
   - Task 1: Create an Object representing a book with properties like title, author, and year, and log the object to the console.
   - Task 2: Access and log the title and author properties of the book object.
2. [Activity 2: Object Methods](#activity-2-object-methods)
   - Task 3: Add a method to the book object that returns a string with the book's title and author, and log the result of calling this method.
   - Task 4: Add a method to the book object that takes a parameter (year) and updates the book's year property, then log the updated object.
3. [Activity 3: Nested Objects](#activity-3-nested-object)
   - Task 5: Create a nested object representing a library with properties like name and books (an array of book objects), and log the library object to the console.
   - Task 6: Access and log the name of the library and the titles of all the books in the library.
4. [Activity 4: The `this` Keyword](#activity-4-the-this-keyword)
   - Task 7: Add a method to the book object that uses the `this` keyword to return a string with the book's title and year, and log the result of calling this method.
5. [Activity 5: Object Iteration](#activity-5-object-iteration)
   - Task 8: Use a `for...in` loop to iterate over the properties of the book object and log each property and its value.
   - Tase 9: Use `Object.keys` and `Object.values` methods to log all the keys and values of the book object.
6. [Feature Request](#feature-request)
   - 1. Book Object Script
   - 2. Library Object Script
   - 3. Object Iteration Script
7. [Achievements](#achievements)

## Activity 1: Object Creation and Access

**Task 1:** Create an Object representing a book with properties like title, author, and year, and log the object to the console.

```javascript
let book = {
    title : "JavaScript with Chai",
    author : "HC",
    year : 2024
};
console.log(book);
//Output : { title: 'JavaScript with Chai', author: 'HC', year: 2024 }
```

**Task 2:** Access and log the title and author properties of the book object.

```javascript
let book = {
    title : "JavaScript with Chai",
    author : "HC",
    year : 2024
};
console.log(book.title); //Output: JavaScript with Chai
console.log(book.author); //Output: HC
```

## Activity 2: Object Methods

**Task 3:** Add a method to the book object that returns a string with the book’s title and author, and log the result of calling this method.

```javascript
let book = {
  title: "Chai Aur Code",
  author: "HC",
  year: 2024,
};

book.getInfo = function () {
  return `${this.title} by ${this.author}`;
};

console.log(book.getInfo());
// Output: Chai Aur Code by HC
```

**Task 4:** Add a method to the book object that takes a parameter (year) and updates the book’s year property, then log the updated object.

```javascript
let book = {
  title: "Chai Aur Code",
  author: "HC",
  year: 2024,
};

book.getInfo = function () {
  return `${this.title} by ${this.author}`;
};

book.updateYear = function (newYear) {
  this.year = newYear;
};
book.updateYear(2020);

console.log(book);
/*
Output:
{
  title: 'Chai Aur Code',
  author: 'HC',
  year: 2020,
  getInfo: [Function (anonymous)],
  updateYear: [Function (anonymous)]
}
*/
```

## Activity 3: Nested Objects

**Task 5:** Create a nested object representing a library with properties like name and books (an array of book objects), and log the library object to the console.

```javascript
let library = {
  name: "City Library",
  books: [
    { title: "Console Busters", author: "MJ", year: 2024 },
    { title: "Chai Aur Code", author: "HC", year: 2024 },
  ],
};

console.log(library);
/*
Output:
{
  name: 'City Library',
  books: [
    { title: 'Console Busters', author: 'MJ', year: 2024 },
    { title: 'Chai Aur Code', author: 'HC', year: 2024 }
  ]
}
*/
```

**Task 6:** Access and log the name of the library and the titles of all the books in the library.

```javascript
let library = {
  name: "City Library",
  books: [
    { title: "Console Busters", author: "MJ", year: 2024 },
    { title: "Chai Aur Code", author: "HC", year: 2024 },
  ],
};

console.log(library.name); // Output: City Library
library.books.forEach((book) => {
  console.log(book.title);
});
// Output:
// Console Busters
// Chai Aur Code
```

## Activity 4: The `this` Keyword

**Task 7:** Add a method to the book object that uses the `this` keyword to return a string with the book’s title and year, and log the result of calling this method.

```javascript
let book = {
  title: "Chai Aur Code",
  author: "HC",
  year: 2024,
};

book.getTitleAndYear = function () {
  return `${this.title} (${this.year})`;
};

console.log(book.getTitleAndYear());
// Output: Chai Aur Code (2024)
```

## Activity 5: Object Iteration

**Task 8:** Use a `for...in` loop to iterate over the properties of the book object and log each property and its value.

```javascript
let book = {
  title: "Chai Aur Code",
  author: "HC",
  year: 2024,
};

book.getInfo = function () {
  return `${this.title} by ${this.author}`;
};

book.updateYear = function (newYear) {
  this.year = newYear;
};
book.updateYear(2020);

for (let key in book) {
  if (book.hasOwnProperty(key)) {
    console.log(`${key}: ${book[key]}`);
  }
}
/*
Output:
title: Chai Aur Code
author: HC
year: 2020
getInfo: function () {

  return `${this.title} by ${this.author}`;

}
updateYear: function (newYear) {

  this.year = newYear;

}
*/
```

**Task 9:** Use `Object.keys(obj)` and `Object.values(obj)` methods to log all the keys and values of the book object.

```javascript
let book = {
  title: "Chai Aur Code",
  author: "HC",
  year: 2024,
};

book.getInfo = function () {
  return `${this.title} by ${this.author}`;
};

book.updateYear = function (newYear) {
  this.year = newYear;
};
book.updateYear(2020);

console.log(Object.keys(book));
// Output: [ 'title', 'author', 'year', 'getInfo', 'updateYear' ]
console.log(Object.values(book));
/* 
Output:
[
  'Chai Aur Code',
  'HC',
  2020,
  [Function (anonymous)],
  [Function (anonymous)]
]
*/
```
## Feature Request:

1. Write a script that creates a book object, adds methods to it, and logs its properties and method results.

2. Create a script that defines a library object containing an array of book objects and logs the library’s details.

3. Write a script that demonstrates iterating over an object’s properties using `for...in` loop and `Object.keys`/`Object.values`.


## Achievements:

By the end of these activities, students will:

- Create and manipulate objects with properties and methods.
- Understand and use the this keyword in object methods.
- Work with nested objects and arrays of objects.
- Iterate over an object’s properties using loops and built-in methods.
