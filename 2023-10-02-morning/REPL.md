# Exploring Node.js REPL (Read-Eval-Print Loop)

### Steps:

- Step 1: Open your terminal or command prompt application.

- Step 2: Type node and press Enter. You should see the Node.js REPL prompt (>) indicating that you are now in the REPL mode.

- Step 3: Basic Usage:
Try typing simple JavaScript expressions and statements, and press Enter after each one. For example:

```js
> 2 + 3
> "Hello, " + "world!"
> const x = 5;
> x * 2
```

- Step 4: Multi-Line Statements:
You can use the . (dot) command to input multi-line statements. This allows you to write code that spans multiple lines without executing it prematurely. For example:

```js

> .editor
```

This will open a new editor mode where you can write multi-line code. Press Ctrl + D to exit the editor and execute the code.

- Step 5: Declaring and Using Functions:
You can define and use functions within the REPL. Try creating a simple function and then calling it:

```js
> function greet(name) {
  return "Hello, " + name + "!";
}
> greet("Alice")
```

- Step 6: Using Special Variables:
The REPL provides special variables such as `_`  to access the results of the last expressions. Try using these special variables:

```js
> 10 + 20
> _
```

- Step 7: Exiting the REPL:
To exit the Node.js REPL, you can use the .exit command or press Ctrl + C twice.

### Conclusion:

The Node.js REPL is a powerful tool for quickly testing and experimenting with JavaScript code. It allows you to interactively explore language features, test ideas, and troubleshoot code snippets without the need for a full-fledged development environment. This lab has provided you with a basic understanding of how to use the Node.js REPL for various tasks.


