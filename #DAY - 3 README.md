# DAY 3: Control Structures

## Table of Contents

1. [Activity 1: If-Else Statements](#activity-1-if-else-statements)
   - Task 1: Number Checks
   - Task 2: Voting Eligibility
2. [Activity 2: Nested If-Else Statements](#activity-2-nested-if-else-statements)
   - Task 3: Find the Largest Among three Numbers
3. [Activity 3: Switch Case](#activity-3-switch-case)
   - Task 4: Day of the Week
   - Task 5: Grade Assignment
4. [Activity 4: Conditional (Ternary) Operator](#activity-4-conditional-ternary-operator)
   - Task 6: Check Even or Odd
5. [Activity 5: Combining Conditions](#activity-5-combining-conditions)
   - Task 7: Check Leap Year or not
6. [Feature Request](#feature-request)
   - 1. Number Check Script
   - 2. Voting Eligibility Script
   - 3. Day of the Week Script
   - 4. Grade Assignment Script
   - 5. Leap Year Check Script
7. [Achievements](#achievements)

## Activity 1: If-Else Statements

**Task 1:** Write a Program to check if a number is positive, negative or zero, and log the result to the console.

```javascript
function numberCheck(n) {
    if(n > 0) {
        console.log("Number is Postive");
    }
    else if(n < 0) {
        console.log("Number is Negative");
    }
    else {
        console.log("Number is zero");
    }
}

numberCheck(10); // Number is Postive
numberCheck(-25); // Number is Negative
numberCheck(0); // Number is zero
```

**Task 2:** Write a Program to check if a person is eligible to vote (age >= 18) and log the result to the console.

```javascript
function checkEligible(age) {
    if(age >= 18) {
        console.log("Eligible for Voting");
    }
    else {
        console.log("Not Eligible for Voting");
    }
}

checkEligible(35); // Eligible for Voting
checkEligible(12); // Not Eligible for Voting
```

## Activity 2: Nested If-Else Statements

**Task 3:** Write a Program to find the largest of three numbers using nested if-else statements.

```javascript
function largeNumber(a,b,c) {
    if(a >= b) {
        if(a >= c) {
            console.log(`${a} is the largest`);
        }
        else {
            console.log(`${c} is the largest`);
        }
    }
    else {
        if(b >=c) {
            console.log(`${b} is the largest`);
        }
        else {
            console.log(`${c} is the largest`);
        }
    }
}

largeNumber(10,20,30); // 30 is the largest
largeNumber(50,20,30); // 50 is the largest
largeNumber(10,80,30); // 80 is the largest
```

## Activity 3: Switch Case

**Task 4:** Write a Program that uses a switch case to determine the day of week based on a number (1-7) and log the day name to the console.

```javascript
function findDays(day) {
    switch(day) {
        case 1: 
            console.log("Sunday");
            break;
        case 2: 
            console.log("Monday");
            break;
        case 3:
            console.log("Tuesday");
            break;
        case 4: 
            console.log("Wednesday");
            break;
        case 5:
            console.log("Thursday");
            break;
        case 6:
            console.log("Friday");
            break;
        case 7:
            console.log("Saturday");
            break;
        default:
            console.log("Invalid Day!, Please Enter a valid day between 1 to 7.");
    }
}
findDays(2); // Monday
findDays(7); // Saturday
```

**Task 5:** Write a Program that uses a switch case to assign a grade ('A', 'B', 'C', 'D', 'F') based on a score and log the grade to the console.

```javascript
function findGrade(n) {
    switch(true) {
        case n >= 90 :
            console.log("Grade : A");
            break;
        case n >= 75 : 
            console.log("Grade : B");
            break;
        case n >= 60 :
            console.log("Grade : C");
            break;
        case n >= 50 :
            console.log("Grade : D");
            break;
        default:
            console.log("Grade : F");
    }
}
findGrade(92); // Grade : A
findGrade(80); // Grade : B
findGrade(45); // Grade : F
```

## Activity 4: Conditional (Ternary) Operator

**Task 6:** Write a Program that uses the ternary operator to check if a number is even or odd and log the result to the console.

```javascript
function EvenOrOdd(n) {
    let ans = (n %2 == 0) ? "Even" : "Odd";
    console.log(ans);
}
EvenOrOdd(20); // Even
EvenOrOdd(17); // odd
```

## Activity 5: Combining Conditions

**Task 7:** Write a Program to check if a year is a leap year using multiple conditions (divisible by 4, but not 100 unless also divisible by 400) and log the result to the console.

```javascript
function isLeapYear(n) {
    if((n%4 == 0 && n%100 != 0) || (n%400 == 0)) {
        console.log(`${n} is a leap year`);
    }
    else {
        console.log(`${n} is not a leap year`);
    }
}
isLeapYear(2024); // 2024 is a leap year
isLeapYear(2017); // 2017 is not a leap year
```

## Feature Request:

1. **Number Check Script:** Write a script that checks if a number is positive, negative, or zero using if-else statements and logs the result.
2. **Voting Eligibility Script:** Create a script to check if a person is eligible to vote based on their age and log the result.
3. **Day of the Week Script:** Write a script that uses a switch case to determine the day of the week based on a number (1-7) and logs the day name.
4. **Grade Assignment Script:** Create a script that uses a switch case to assign a grade based on a score and logs the grade.
5. **Leap Year Check Script:** Write a script that checks if a year is a leap year using multiple conditions and logs the result.

## Achievements:

By the end of these activities, students will:

- Implement and understand basic if-else control flow.
- Use nested if-else statements to handle multiple conditions.
- Utilize switch cases for control flow based on specific values.
- Apply the ternary operator for concise condition checking.
- Combine multiple conditions to solve more complex problems.
