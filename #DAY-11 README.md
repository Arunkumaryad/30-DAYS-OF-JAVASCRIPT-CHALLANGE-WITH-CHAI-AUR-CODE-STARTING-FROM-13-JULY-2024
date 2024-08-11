# Day 11: Promises and Async/Await


## Table of Contents

1. [Activity 1: Undrstanding Promises](#activity-1-understanding-promises)
   - Task 1: Create a Promise that Resolves
   - Task 2: Create a Promise that Rejects
2. [Activity 2: Chaining Promises](#activity-2-chaining-promises)
   - Task 3: Sequence of Promises
3. [Activity 3: Using Asyns/Await](#activity-3-using-async-await)
   - Task 4: Async Function with Resolved Promise
   - Task 5: Async Function with Rejected Promise
4. [Activity 4: Fetching Data from an API](#activity-4-fetching-data-from-an-api)
   - Task 6: Fetch API with Promises
   - Task 7: Fetch API with Async/Await
5. [Activity 5: Concurrent Promises](#activity-5-concurrent-promises)
   - Task 8: Using `Promise.all`
   - Task 9: Using `Promise.race`
6. [Feature Request](#feature-request)
7. [Achievements](#achievements)

## Activity 1: Understanding Promises

**Task 1:** Create a promise that resolves with a message after a 2-second timeout and log the message to the console.

```javascript
const PromiseResolve = new Promise((res) => {
    setTimeout(() => {
        res("Promise resolved after 2 sec");
    },2000);
});
PromiseResolve.then((message) => {
    console.log(message); // Promise resolved after 2 sec
});
```

**Task 2:** Create a promise that rejects with an error message after a 2-second timeout and handle the error using `.catch().`

```javascript
const PromiseResolve = new Promise((_,reject) => {
    setTimeout(() => {
        reject("Promise rejected after 2 sec");
    },2000);
});
PromiseResolve.catch((err) => {
    console.log(err); // Promise rejected after 2 sec
});
```

## Activity 2: Chaining Promises

**Task 3:** Create a sequence of promises that simulate fetching data from a server. Chain the promises to log messages in a specific order.

```javascript
const fetchData = (data, delay) => {
  return new Promise((resolve) => {
    setTimeout(() => {
      resolve(data);
    }, delay);
  });
};

fetchData("Fetching data from server 1", 1000)
  .then((message) => {
    console.log(message); // Fetching data from server 1
    return fetchData("Fetching data from server 2", 1000);
  })
  .then((message) => {
    console.log(message); // Fetching data from server 2
    return fetchData("Fetching data from server 3", 1000);
  })
  .then((message) => {
    console.log(message); // Fetching data from server 3
  });
```


## Activity 3: Using Async/Await

**Task 4:** Write an async function that waits for a promise to resolve and then logs the resolved value.

```javascript
const asyncFunction = async () => {
    const promise = new Promise((res) => {
     setTimeout(() => {
         res("Promise resolved from Async Functions");
    },2000);
 });
 const ans = await promise;
 console.log(ans); //Promise resolved from Async Functions
};
asyncFunction();
```

**Task 5:** Write an async function that handles a rejected promise using try-catch and logs the error message.

```javascript
const asyncFunction = async () => {
    const promise = new Promise((_, reject) => {
     setTimeout(() => {
         reject("Promise rejected from Async Functions");
    },2000);
 });
 try {
     const ans = await promise;
     console.log(ans);
 }
 catch(err) {
     console.error(err); //Promise rejected from Async Functions
 }
};
asyncFunction();
```

## Activity 4: Fetching Data From An API

**Task 6:** Use the fetch API to get data from a public API and log the response data to the console using promises.

```javascript
fetch("https://jsonplaceholder.typicode.com/posts")
  .then((response) => response.json())
  .then((data) => {
    console.log(data);
  })
  .catch((error) => {
    console.error("Error fetching data:", error);
  });

/*
[
  {
    "userId": 1,
    "id": 1,
    "title": "sunt aut facere repellat provident occaecati excepturi optio reprehenderit",
    "body": "quia et suscipit\nsuscipit recusandae consequuntur expedita et cum\nreprehenderit molestiae ut ut quas totam\nnostrum rerum est autem sunt rem eveniet architecto"
  },
  {
    "userId": 1,
    "id": 2,
    "title": "qui est esse",
    "body": "est rerum tempore vitae\nsequi sint nihil reprehenderit dolor beatae ea dolores neque\nfugiat blanditiis voluptate porro vel nihil molestiae ut reiciendis\nqui aperiam non debitis possimus qui neque nisi nulla"
  }
]
*/
```

**Task 7:** Use the fetch API to get data from a public API and log the response data to the console using async/await.

```javascript
const fetchDataAsync = async () => {
  try {
    const response = await fetch("https://jsonplaceholder.typicode.com/posts");
    const data = await response.json();
    console.log(data);
  } catch (error) {
    console.error("Error fetching data:", error);
  }
};

fetchDataAsync();
/*
[
  {
    "userId": 1,
    "id": 1,
    "title": "sunt aut facere repellat provident occaecati excepturi optio reprehenderit",
    "body": "quia et suscipit\nsuscipit recusandae consequuntur expedita et cum\nreprehenderit molestiae ut ut quas totam\nnostrum rerum est autem sunt rem eveniet architecto"
  },
  {
    "userId": 1,
    "id": 2,
    "title": "qui est esse",
    "body": "est rerum tempore vitae\nsequi sint nihil reprehenderit dolor beatae ea dolores neque\nfugiat blanditiis voluptate porro vel nihil molestiae ut reiciendis\nqui aperiam non debitis possimus qui neque nisi nulla"
  }
]
*/
```

## Activity 5: Concurrent Promises

**Task 8:** Use `Promise.all` to wait for multiple promises to resolve and then log all their values. Task 9: Use Promise.race to log the value of the first promise that resolves among multiple promises.
```javascript
// Task 8
const promise1 = new Promise((resolve) =>
  setTimeout(resolve, 1000, "First promise")
);
const promise2 = new Promise((resolve) =>
  setTimeout(resolve, 2000, "Second promise")
);
const promise3 = new Promise((resolve) =>
  setTimeout(resolve, 3000, "Third promise")
);

Promise.all([promise1, promise2, promise3]).then((values) => {
  console.log("All promises resolved:", values);
});


```

**Task 9:** Use `promise.race` to log the value of the first promise that resolves among multiple promises.

```javascript
// Task 9
Promise.race([promise1, promise2, promise3]).then((value) => {
  console.log("First promise resolved:", value);
});

First promise resolved: First promise
All promises resolved: [ 'First promise', 'Second promise', 'Third promise' ]
```

## Feature Request

1. **Promise Creation Script:** Write a script that demonstrates creating and handling promises, including both resolved and rejected states.

2. **Promise Chaining Script:** Create a script that chains multiple promises and logs messages in a specific sequence.

3. **Async/Await Script:** Write a script that uses async/await to handle promises and includes error handling with try-catch.

4. **API Fetch Script:** Create a script that fetches data from a public API using both promises and async/await, and logs the response data.

5. **Concurrent Promises Script:** Write a script that uses `Promise.all` and `Promise.race` to handle multiple promises concurrently and logs the results.

## Achievements

By completing these activities, students will:


- Understand and create promises, including handling resolved and rejected states.
- Chain multiple promises to perform sequential asynchronous operations.
- Use async/await to handle asynchronous code more readably.
- Fetch data from public APIs using both promises and async/await.
- Manage multiple concurrent promises using `Promise.all` and `Promise.race`.
