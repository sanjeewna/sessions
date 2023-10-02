# `var`, `let`, and `const`

In JavaScript, `var`, `let`, and `const` are used to declare variables. They have different scoping rules and behaviors. Understanding the differences between them is important for writing clean and predictable code:

1. **`var`**:

   - **Function Scope**: Variables declared with `var` are function-scoped, meaning they are visible throughout the entire function in which they are defined.

   - **Hoisting**: Variables declared with `var` are hoisted to the top of their containing function or global scope. This means you can use a `var` variable before it's declared, but it will have an initial value of `undefined`.

   - **Redeclaration**: You can redeclare a variable using `var` in the same scope without any error.

   ```javascript
   function example() {
     var x = 10;
     if (true) {
       var x = 20; // This reassigns the outer 'x' variable
       console.log(x); // Outputs 20
     }
     console.log(x); // Outputs 20
   }
   ```

   - **Global Scope**: If declared outside of a function, `var` variables become global variables.

   ```javascript
   var globalVar = "I'm a global variable";
   ```

2. **`let`**:

   - **Block Scope**: Variables declared with `let` are block-scoped, meaning they are confined to the block in which they are defined. This is typically a pair of curly braces `{}`.

   - **Hoisting**: Variables declared with `let` are also hoisted, but they are not initialized. You cannot use a `let` variable before it's declared, unlike `var`.

   - **No Redeclaration**: You cannot redeclare a variable in the same scope using `let`.

   ```javascript
   function example() {
     let x = 10;
     if (true) {
       let x = 20; // This creates a new 'x' variable within the block scope
       console.log(x); // Outputs 20
     }
     console.log(x); // Outputs 10 (the outer 'x' remains unchanged)
   }
   ```

3. **`const`**:

   - **Block Scope**: Like `let`, variables declared with `const` are block-scoped.

   - **Hoisting**: Variables declared with `const` are also hoisted but, similar to `let`, they are not initialized. You cannot use a `const` variable before it's declared.

   - **Constant Value**: `const` variables are constant, meaning their values cannot be reassigned once they are set.

   ```javascript
   const pi = 3.14159;
   pi = 4; // This will result in an error because 'pi' is a constant
   ```

   - **Object Mutation**: While you cannot reassign a `const` variable, if it holds an object or array, you can still modify the object's properties or elements. The reference to the object or array remains constant, not the content.

   ```javascript
   const colors = ["red", "green", "blue"];
   colors.push("orange"); // This is allowed
   ```

In modern JavaScript, it's recommended to use `let` for variables that may change their values and `const` for variables that should remain constant. `var` is rarely used in modern code due to its unpredictable scoping behavior and hoisting. Using `let` and `const` helps improve code clarity and predictability.