# Creating and Using Custom Modules

### Introduction:

In this task, you will learn how to create your own custom modules in Node.js and use them within your scripts. Node.js modules allow you to organize your code into reusable components, promoting modularity and maintainability.

###  Prerequisites:

Node.js installed on your machine.

### Steps:

- Step 1: Create a new directory `custom-modules` and Open Visual Studio Code from inside the folder.

- Step 2: Create two new files named `mathOperations.js` and `app.js` in the directory.
 
- Step 3: Open the `mathOperations.js` file and define a custom module that exports four functions:

```javascript
// mathOperations.js

// Function to add two numbers
function add(a, b) {
  return a + b;
}

// Function to subtract two numbers
function subtract(a, b) {
  return a - b;
}

// Function to multiply two numbers
function multiply(a, b) {
  return a * b;
}

// Function to divide two numbers
function divide(a, b) {
  if (b === 0) {
    throw new Error("Division by zero is not allowed.");
  }
  return a / b;
}

// Export the functions
module.exports = {
  add,
  subtract,
  multiply,
  divide,
};
```

- Step 4: Use the Custom Module:
Open the `app.js` file and require the custom module you created in the previous step. Use the exported functions to perform mathematical operations:

```javascript
// app.js

// Import the mathOperations module
const math = require('./mathOperations');

// Use the functions from the imported module
const resultAddition = math.add(10, 5);
console.log(`Addition: ${resultAddition}`);

const resultSubtraction = math.subtract(10, 5);
console.log(`Subtraction: ${resultSubtraction}`);

const resultMultiplication = math.multiply(10, 5);
console.log(`Multiplication: ${resultMultiplication}`);

const resultDivision = math.divide(10, 5);
console.log(`Division: ${resultDivision}`);
```

- Step 5: Save and Close the Files:
Save the changes you made to both `mathOperations.js` and `app.js`.

- Step 6: Run the Script:
Execute the `app.js` script using the Node.js runtime:

```sh
node app.js
```
You will see the results of the mathematical operations displayed in the terminal.

- This example demonstrates how to create a module (`mathOperations.js`) that exports functions for common mathematical operations and how to import and use those functions in another file (`app.js`) within the same project. You can extend this concept to create and use modules for various functionalities in your Node.js applications.




