
# Lecture 6

[Back](../README.md)

## What We Learned in JavaScript – Lecture 6

In this lecture, we covered:

* Basic output using `console.log` and `alert`
* JavaScript data types
* Declaring variables using `var`, `let`, and `const`

---

### Output in JavaScript

```javascript
console.log("welcome to js");
alert("welcome to js");
```

---

### JavaScript Data Types

```javascript
// string : any character in double or single quotes
let name = "John";

// number : any number floating or integer
let age = 25;

// boolean : true or false
let isStudent = true;

// list : many values in square brackets
let scores = [1, 2, 3, 4];

// object : many values in curly brackets
let student = {name: "john", age: 20};

// null : no value
let nothing = null;

// undefined : no value assigned
let unknown;

// NaN : not a number
let result = 0 / "hello";
```

---

### Declaring Variables in JavaScript

#### Using `var`

```javascript
// var : variable that can be changed
var studentName = "john doe"; // string
console.log(studentName);

studentName = "Mohammad";
console.log(studentName);
```

#### Using `let`

```javascript
// let : variable that can be changed, but has block scope
let studentAge = 20; // number
console.log(studentAge);

studentAge = 25;
console.log(studentAge);
```

#### Using `const`

```javascript
// const : variable that cannot be changed
const newData = "new data"; // string
console.log(newData);

// newData = "new data 2"; // ❌ this will cause an error
// console.log(newData);   // uncommenting this line will cause an error
```
