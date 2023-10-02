# Activity 2

> If there's not enough time during the class, kindly complete the activity on your own afterward.


This activity is designed to introduce you to Visual Studio Code (VSCode), working with folders and files, running Node.js scripts, and creating and using modules:

### Task 1/7: Installing and Configuring VSCode

In this task, you will download and install Visual Studio Code and configure it for a smoother workflow.

1. Download and install Visual Studio Code from [https://code.visualstudio.com/](https://code.visualstudio.com/).
2. During installation, make sure 
  - to check the option to add VSCode to your system's PATH
  - add VSCode to your context menu for easier access.

### Task 2/7: Getting Familiar with VSCode Basics

In this task, you will become familiar with essential VSCode features.

1. Create a new directory `vscode-basics` and open Visual Studio Code from inside the folder.
2. Create a new file name `hello.txt` inside `vscode-basics`.
3. Create a new folder `my-folder` inside `vscode-basics`. Do not use spaces in the folder name, e.g., `my-folder` instead of `my folder`.
4. Open a terminal within VSCode and ensure that the terminal is pointing to the `my-folder` directory.

### Task 3/7: Running Node.js Scripts in VSCode

In this task, you will learn how to run Node.js scripts directly from within VSCode.

1. Open `vscode-basics` folder in VSCode.
2. Create a new JavaScript file (e.g., `app.js`) inside the folder.
3. Write a simple Node.js script in `app.js`, such as printing "Hello, World!" to the console.
```javascript
// Print "Hello, World!" to the console
console.log("Hello, World!");
```
4. Open the integrated terminal in VSCode in the folder containing your `app.js` file.
5. Run the Node.js script using the terminal by entering `node app.js`.

### Task 4/7: Creating and Using Your Own Module

In this task, you will learn how to create, export, and import your own Node.js module.

1. Create a new JavaScript file (e.g., `math.js`) in the same folder.
2. In `math.js`, define a simple math function (e.g., `add`) and export it using `module.exports`.
```javascript
// math.js
function add(a, b) {
    return a + b;
}
module.exports = { add };
```

3. Create another JavaScript file (e.g., `main.js`) in the same folder.
4. In `main.js`, import the `math` module using `require` and use the `add` function.
```javascript
// main.js
const math = require('./math'); // Assuming both files are in the same folder
const result = math.add(2, 3);
console.log(result);
```

5. Use the integrated terminal to run `main.js` with Node.js (`node main.js`) and observe the output.

### Task 5/7:

1. [Creating and Using Node.js Scripts](./node-scipts.md)
2. [Creating and Using Custom Modules](./modules.md)

### Task 6/7:

Try to use ChatGPT to request examples demonstrating how to utilize custom modules in Node.js

### Task 7/7
3. Remember to reflect on this activity in the reflection journal **(At home)**
