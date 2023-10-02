# Creating and Using Node.js Scripts

### Introduction:

In this task, you will learn how to create and use Node.js scripts. Node.js allows you to execute JavaScript files as scripts, making it possible to automate tasks, build utilities, and perform various operations using the power of JavaScript.

### Prerequisites:

- Node.js installed on your machine.

### Lab Steps:

- Step 1: Create a new directory `node-scripts` and Open Visual Studio Code from inside the folder.
- Step 2: Create a new file named `greeting.js` in the `node-scriptsb` directory. You'll write your script in this file.
- Step 3: Open the `greeting.js` file.
- Step 4: Inside the `greeting.js` file, write a regular function that generates a greeting message using the provided name:

```shell
// greeting.js
function generateGreeting(name) {
  return "Hello, " + name + "!";
}

const personName = "Alice";
const greetingMessage = generateGreeting(personName);
console.log(greetingMessage);
```

- Step 5: Save the changes you made to the greeting.js file.
- Step 6: 
- Open the integrated terminal in VSCode in the folder containing your `greeting.js` file.
- Run the Node.js script using the terminal by entering:

```shell
node greeting.js
```

You should see the output: `Hello, Alice!`.

- Step 7: Modify and Rerun:
Experiment with modifying the personName variable and re-run the script to see how the output changes:

```shell
const personName = "Bob";
const greetingMessage = generateGreeting(personName);
console.log(greetingMessage);
```

### Conclusion:

You've successfully created a Node.js script using regular functions. This task has shown you how to create a simple script that generates a greeting message using a regular function and runs it using the Node.js runtime.

###  Optional Further Steps:

- Experiment with adding more functions to the script, performing different operations.
- Create a new script file for a different task and practice.





