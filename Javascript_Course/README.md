# Javascript

**JavaScript is a powerful language that can help you build interactive websites**

## Basics of Javascript
- Comments
- Variables
- Data Types
- Operators
- Control Structures
  - Conditional Statements
  - Loops
  - Control Flow Statements
- Functions
- Objects
- Arrays
- Events


## Comments
####  Single-line Comments
Use **//** to add a comment on a single line.

```javascript
// This is a single-line comment
let x = 5; // This comment follows code on the same line
```

#### Multi-line Comments
Use **\/\* \*/** to add comments that span multiple lines.
```javascript
/*
  This is a multi-line comment.
  It can span multiple lines.
*/
let y = 10;
```

## console.log

console.log is a function in JavaScript that prints messages to the console. It's widely used for debugging purposes and for displaying information during development.


```javascript
console.log("Hello, World");
```


#### console.error: Prints error messages.

```javascript
console.error("This is an error message");
```


#### console.warn: Prints warning messages.

```javascript
console.warn("This is a warning message");
```
#### console.info: Prints informational messages.


```javascript
console.info("This is an informational message");
```

#### console.table: Displays data as a table.

```javascript
console.table(["Omar","Adel","Shalaan"]);
```
#### Styling Console
```javascript
console.log("%cHello, %cWorld", "color:red; font-size: 30px", "color:blue; font-size: 30px");
```


## Data Types

```javascript
console.log("Omar Adel Shalaan"); // Omar Adel Shalaan
console.log(typeof "Omar Adel Shalaan"); // String
console.log(typeof 5000); // Number
console.log(typeof 10.5); // Number
console.log(typeof [1, 2, 3]); // Array => Object
console.log(typeof ["Omar","Adel","Shalaan"]); // Object
console.log(typeof { name: "Omar", age: 45, country: "Eg" }); // Object
console.log(typeof true); // Boolean
console.log(typeof false); // Boolean
console.log(typeof undefined); // undefined
console.log(typeof null); // Object
```

## Variables
variables are used to store and manipulate data. You can declare variables using **let**, **const**, or **var**

- #### let
  - Usage: Allows you to change the variable’s value.
  - Scope: Block-scoped (limited to the block where it is defined).
    ```javascript
    let name = "Alice";
    name = "Bob"; // You can reassign the value
    ```
- #### const
  - Usage: Defines a constant variable whose value cannot be changed.
  - Scope: Block-scoped.
    ```javascript
    const pi = 3.14;
    // pi = 3.1415; // This will cause an error because you cannot reassign a constant
    ```

- #### var
  - Usage: Used in older code; allows you to change the variable’s value.
  - Scope: Function-scoped (or globally if declared outside a function). Avoid using var in modern code.
    ```javascript
    var city = "New York";
    city = "Los Angeles"; // You can reassign the value
    ```
#### Examples
```javascript
let age = 30; // A variable that can change
const birthYear = 1994; // A constant variable

// Function to demonstrate variable scope
function showScope() {
    var insideVar = "I'm inside a function"; // Function-scoped
    console.log(insideVar);
}

showScope();
console.log(insideVar); // This will cause an error because insideVar is not defined outside the function
```

## Operators
- #### Arithmetic Operators: +, -, *, /, %, ++, --
- #### Comparison Operators: ==, \=\==, !=, !=\=, >, <, >=, <=
- #### Logical Operators: &&, ||, !
- #### Assignment Operators: =, +=, -=, *=, /=

### Arithmetic Operators

- #### Addition (+)
```javascript
let a = 5;
let b = 3;
let sum = a + b;
console.log(sum); // Output: 8
```
- #### Subtraction (-)
```javascript
let difference = a - b;
console.log(difference); // Output: 2
```
- #### Multiplication (*)
```javascript
let product = a * b;
console.log(product); // Output: 15
```
- #### Division (/)
```javascript
let quotient = a / b;
console.log(quotient); // Output: 1.666...
```
- #### Modulus (%)
```javascript
let remainder = a % b;
console.log(remainder); // Output: 2
```
- #### Increment (++)
```javascript
let count = 0;
count++;
console.log(count); // Output: 1
```
- #### Decrement (--)
```javascript
let count = 1;
count--;
console.log(count); // Output: 0
```

### Comparison Operators

- #### Equal to (==)
  Checks if two values are equal, performing type conversion if necessary.
```javascript
console.log(5 == '5'); // Output: true
```
- #### Strict Equal to (===)
  Checks if two values are equal and of the same type.
```javascript
console.log(5 === '5'); // Output: false
console.log(5 === 5);   // Output: true
```
- #### Not Equal to (!=)
  Checks if two values are not equal, performing type conversion if necessary.
```javascript
console.log(5 != '5'); // Output: false
```
- #### Strict Not Equal to (!==)
  Checks if two values are not equal or not of the same type.
```javascript
console.log(5 !== '5'); // Output: true
console.log(5 !== 5);   // Output: false
```
- #### Greater Than (>)
```javascript
console.log(5 > 3); // Output: true
```
- #### Less Than (<)
```javascript
console.log(5 < 3); // Output: false
```
- #### Greater Than or Equal to (>=)
```javascript
console.log(5 >= 5); // Output: true
```
- #### Less Than or Equal to (<=)
```javascript
console.log(5 <= 3); // Output: false
```

### Logical Operators

- #### Logical AND (&&)
```javascript
console.log(true && false); // Output: false
console.log(true && true);  // Output: true
```
- #### Logical OR (||)
```javascript
console.log(true || false); // Output: true
console.log(false || false); // Output: false
```
- #### Logical NOT (!)
```javascript
console.log(!true);  // Output: false
console.log(!false); // Output: true
```

### Assignment Operators

- #### Assignment (=)
```javascript
let x = 10;
console.log(x); // Output: 10
```

- #### Addition Assignment (+=)
```javascript
x += 5; // Equivalent to x = x + 5
console.log(x); // Output: 15
```
- #### Subtraction Assignment (-=)
```javascript
x -= 3; // Equivalent to x = x - 3
console.log(x); // Output: 12
```
- #### Multiplication Assignment (*=)
```javascript
x *= 2; // Equivalent to x = x * 2
console.log(x); // Output: 24
```
- #### Division Assignment (/=)
```javascript
x /= 4; // Equivalent to x = x / 4
console.log(x); // Output: 6
```
- #### Modulus Assignment (%=)
```javascript
x %= 3; // Equivalent to x = x % 3
console.log(x); // Output: 0
```


## Control Structures
**Conditional statements allow you to execute code based on specific conditions.**

### Conditional Statements
- #### if Statement
  Executes a block of code if a specified condition is true.
```javascript
let age = 18;

if (age >= 18) {
    console.log("You are an adult.");
}
```
- #### if...else Statement
  Executes one block of code if a condition is true, and another block if it is false.
```javascript
let age = 16;

if (age >= 18) {
    console.log("You are an adult.");
} else {
    console.log("You are a minor.");
}
```
- #### if...else if...else Statement
  Checks multiple conditions, executing code for the first true condition, and a default block if none of the conditions are true.
```javascript
let score = 85;

if (score >= 90) {
    console.log("Grade: A");
} else if (score >= 80) {
    console.log("Grade: B");
} else if (score >= 70) {
    console.log("Grade: C");
} else {
    console.log("Grade: D or below");
}
```
- #### switch Statement
  Evaluates an expression and executes code based on matching cases. It's useful when you have multiple conditions to check against a single value.
```javascript
let day = "Monday";

switch (day) {
    case "Monday":
        console.log("Start of the workweek!");
        break;
    case "Friday":
        console.log("Weekend is near!");
        break;
    case "Saturday":
    case "Sunday":
        console.log("It's the weekend!");
        break;
    default:
        console.log("Just another day");
}
```
## Loops
**Loops are used to execute a block of code repeatedly under certain conditions.**
- #### for Loop
  Executes a block of code a specific number of times.
```javascript
for (let i = 0; i < 5; i++) {
    console.log(i); // Output: 0, 1, 2, 3, 4
}
```
- #### while Loop
  Executes a block of code as long as a condition is true. It may not execute at all if the condition is false initially.
```javascript
let i = 0;

while (i < 5) {
    console.log(i); // Output: 0, 1, 2, 3, 4
    i++;
}
```
- #### do...while Loop
  Executes a block of code at least once, and then continues executing as long as a condition is true.
```javascript
let i = 0;

do {
    console.log(i); // Output: 0, 1, 2, 3, 4
    i++;
} while (i < 5);
```
## Control Flow Statements
**Control flow statements alter the flow of a loop or conditional execution.**
- #### break
  Exits a loop or switch statement prematurely.
```javascript
for (let i = 0; i < 10; i++) {
    if (i === 5) {
        break;
    }
    console.log(i); // Output: 0, 1, 2, 3, 4
}
```
- #### continue
  Skips the current iteration of a loop and continues with the next iteration.
```javascript
for (let i = 0; i < 10; i++) {
    if (i % 2 === 0) {
        continue;
    }
    console.log(i); // Output: 1, 3, 5, 7, 9
}
```
- #### return
  Exits from a function and optionally returns a value.
```javascript
function multiply(a, b) {
    return a * b;
}

let result = multiply(3, 4);
console.log(result); // Output: 12
```

## Functions
  Functions in JavaScript are reusable blocks of code designed to perform a specific task. They can take inputs, process them, and return outputs.


- #### Function Declaration
  A function declaration defines a named function that can be called later in the code.

```javascript
function functionName(parameters) {
    // code to be executed
    return value; // optional
}
```
- #### Example
```javascript
function greet(name) {
    return `Hello, ${name}!`;
}

console.log(greet("Alice")); // Output: Hello, Alice!
```
- #### Parameters and Arguments
  Functions can accept parameters, which are placeholders for the values you pass in (arguments) when calling the function.

**Default Parameters**
You can provide default values for parameters in case no argument is passed.
```javascript
function greet(name = "Guest") {
    return `Hello, ${name}!`;
}

console.log(greet()); // Output: Hello, Guest!
```

- #### Returning Values
  Functions can return values to the caller using the **return** statement. If no return statement is used, the function returns **undefined** by default.

```javascript
function calculateArea(radius) {
    return Math.PI * radius * radius;
}

let area = calculateArea(5);
console.log(area); // Output: 78.53981633974483
```

- #### Function Scope
  Variables declared inside a function are local to that function and cannot be accessed from outside.
```javascript
function testScope() {
    let localVariable = "I am local";
    console.log(localVariable); // Output: I am local
}

testScope();
console.log(localVariable); // Error: localVariable is not defined
```
## Objects
  objects are fundamental data structures that allow you to group and manage related data and functions. An object is a collection of properties, where each property is a key-value pair.

### Creating Objects 

- #### Object Literal Notation
  The most common way to create an object is using object literal notation.
```javascript
let person = {
    name: "John",
    age: 30,
    isEmployed: true
};
```

- #### Using the new Object() Syntax
  You can also create objects using the new Object() constructor.
```javascript
let person = new Object();
person.name = "John";
person.age = 30;
person.isEmployed = true;
```

### Accessing Object Properties 
  You can access object properties using dot notation or bracket notation.

- #### Dot Notation
```javascript
console.log(person.name); // Output: John
```

- #### Bracket Notation

```javascript
console.log(person["age"]); // Output: 30

let property = "isEmployed";
console.log(person[property]); // Output: true
```

### Modifying Object Properties
  You can modify the properties of an object using either dot or bracket notation.
- #### Dot Notation

```javascript
person.name = "Jane";
console.log(person.name); // Output: Jane
```

- #### Bracket Notation

```javascript
person["age"] = 31;
console.log(person["age"]); // Output: 31
```

### Adding and Deleting Properties

- #### Adding Properties

```javascript
person.job = "Developer";
console.log(person.job); // Output: Developer
```

- #### Deleting Properties

```javascript
delete person.job;
console.log(person.job); // Output: undefined
```
### Object Methods
  Objects can contain methods, which are functions associated with the object.


- #### Defining Methods

```javascript
let person = {
    name: "John",
    age: 30,
    greet: function() {
        return `Hello, my name is ${this.name}.`;
    }
};

console.log(person.greet()); // Output: Hello, my name is John.
```

- #### Shorthand Method Definition

```javascript
let person = {
    name: "John",
    age: 30,
    greet() {
        return `Hello, my name is ${this.name}.`;
    }
};

console.log(person.greet()); // Output: Hello, my name is John.
```
### this Keyword
  The this keyword refers to the object that the method is called on. It is used to access properties and methods within the same object.

```javascript
let person = {
    name: "John",
    age: 30,
    describe() {
        return `${this.name} is ${this.age} years old.`;
    }
};

console.log(person.describe()); // Output: John is 30 years old.
```

### Object Constructor Function
  Object Constructor Function

```javascript
function Person(name, age) {
    this.name = name;
    this.age = age;
    this.greet = function() {
        return `Hello, my name is ${this.name}.`;
    };
}

let person1 = new Person("John", 30);
let person2 = new Person("Jane", 25);

console.log(person1.greet()); // Output: Hello, my name is John.
console.log(person2.greet()); // Output: Hello, my name is Jane.
```

### Object.create() Method
- #### 
  The Object.create() method creates a new object with the specified prototype object and properties.
```javascript
let protoPerson = {
    greet() {
        return `Hello, my name is ${this.name}.`;
    }
};

let person = Object.create(protoPerson);
person.name = "John";
console.log(person.greet()); // Output: Hello, my name is John.
```

## Arrays
Arrays in JavaScript are a type of object used for storing ordered collections of values. They provide a way to work with lists of items, whether they are numbers, strings, or other objects.

### Creating Arrays
- #### Array Literal Notation
The most common way to create an array is using the array literal notation.
```javascript
let fruits = ["apple", "banana", "cherry"];
```

- #### Using the Array Constructor
You can also create arrays using the Array constructor.
```javascript
let numbers = new Array(1, 2, 3, 4);
let emptyArray = new Array(5); // Creates an array with 5 undefined elements [ <5 empty items> ]
```
### Accessing and Modifying Elements
- #### Accessing Elements
You access array elements using their index, starting from 0.
```javascript
let firstFruit = fruits[0]; // "apple"
let secondFruit = fruits[1]; // "banana"
```

- #### Modifying Elements

```javascript
fruits[1] = "blueberry";
console.log(fruits); // ["apple", "blueberry", "cherry"]
```

### Array Properties and Methods


- #### Adding Elements

1. - #### Using push()
Adds one or more elements to the end of an array.
```javascript
fruits.push("date");
console.log(fruits); // ["apple", "blueberry", "cherry", "date"]
```

2. - #### Using unshift()
Adds one or more elements to the beginning of an array.
```javascript
fruits.unshift("apricot");
console.log(fruits); // ["apricot", "apple", "blueberry", "cherry", "date"]
```

- #### Removing Elements

1. - #### Using pop()
Removes the last element from an array and returns it.
```javascript
let lastFruit = fruits.pop();
console.log(lastFruit); // "date"
console.log(fruits); // ["apricot", "apple", "blueberry", "cherry"]
```

2. - ####  Using shift()
Removes the first element from an array and returns it.

```javascript
let firstFruitRemoved = fruits.shift();
console.log(firstFruitRemoved); // "apricot"
console.log(fruits); // ["apple", "blueberry", "cherry"]
```




# Reference
- ### [Free code Camp](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures)
