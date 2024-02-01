# Javascript Interview Question and Answers 2024

- **What is JavaScript and what is it used for?**

  > JavaScript is a programming language used for creating interactive and dynamic websites. It can also be used for server-side development with Node.js.

- **What are the different data types in JavaScript?**
  > DataTypes in javascript can be broadly categorized into 2 main types those are Primitive DataTypes and Composite (Non-primitive) DataTypes.
- **What is the difference between `primitive` and `composite` data types in js?**
 <table border="0">
 <tr align="center">
 <td>Primitive</td>
 <td>Composite</td>
 </tr>
 <tr align="center">
 <td ><b>(Immutable)</b><br> Primitive data types are immutable, meaning their values cannot be changed after creation.<br>
 (example)<br>if you have a string and modify it, you are creating a new string rather than modifying the original.
 </td><td><b>(Mutable)</b><br>Composite data types are mutable, meaning their values can be changed after creation. <br>
 (example) <br>
 if you modify an object or array, you are modifying the original object or array.
 </td>
 </tr>
 <!-- <tr align="center">
 <td>Primitive</td>
 <td>Composite</td>
 </tr> -->
 <tr align="center"><td><b>(Stored by Value)</b><br>
 Primitive values are stored directly in memory, and when assigned to a variable, the actual value is stored.
 </td><td><b>(Stored by Reference)</b><br>
 Composite values are stored by reference, and when assigned to a variable instead of the actual value a memory address is stored.
 </td></tr>
 <!-- <tr align="center">
 <td>Primitive</td>
 <td>Composite</td>
 </tr> -->
 <tr align="center"><td><b>(Copy by Value)</b><br>
 When assigned to a new variable or passed as a parameter, primitive values are copied by value. Modifying the copied value does not affect the original.
 </td><td><b>(Copy by Reference)</b><br>
When assigned to a new variable or passed as a parameter, composite values are copied by reference.
Modifying the copied reference affect the original object or array. 
 </td></tr>
 </table>

- **How do you declare a variable in JavaScript?**
  > In Javascript `var`, `let` and `const` keywords is used to declare a variable.
- **What is the difference between `let`, `const`, and `var` in JavaScript?**
<table border="0">
    <thead>
      <tr>
        <th>Difference</th>
        <th><code>var</code></th>
        <th><code>let</code></th>
        <th><code>const</code></th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Scope</td>
        <td>Function-scoped</td>
        <td>Block-scoped</td>
        <td>Block-scoped</td>
      </tr>
      <tr>
        <td>Hoisting</td>
        <td>Hoisted (initialized with <code>undefined</code>)</td>
        <td>Hoisted (temporal dead zone)</td>
        <td>Hoisted (temporal dead zone)</td>
      </tr>
      <tr>
        <td>Reassignment</td>
        <td>Can be reassigned</td>
        <td>Can be reassigned</td>
        <td>Cannot be reassigned</td>
      </tr>
      <tr>
        <td>Redeclaration</td>
        <td>Can be redeclared</td>
        <td>Cannot be redeclared</td>
        <td>Cannot be redeclared</td>
      </tr>
    </tbody>
  </table>

  - **What is scope in javascript?**
    >Scope in javascript refers to the area where a variable can be accessed.
  - **What are the different types of scope in javascript?**
    >There are 4 types of scope in javascript. These are global scope, local scope (function scope), block scope and lexical scope.
  - **Explain the different types of scope in javascript?** 
    - Global Scope
      >Variables declared outside of any function or block have global scope. They are accessible from anywhere in the code, including functions and blocks.
    - Local Scope (Function Scope)
      >Variables declared inside a function have local scope. They are only accessible within that function.
    - Block Scope (introduced by `let` and `const`)
      >Variables declared with `let` and `const` have block scope. They are only accessible within the block (enclosed by curly braces `{}`) where they are defined.
    - Lexical Scope (Closure)
      >Where a function can access variables from its outer function is called lexical scope.
  - **What is hoisting in javascript?**
    >Hoisting in javascript is a process that happens during the creation/compilation phase, where variable and function declaration are moved to the top of their scope. This allows you to use variables and functions before they are declared in the code.
  - **How does hoisting work with variable declarations?**
    >Variable declarations using `var` are hoisted to the top of their containing scope and they are initialized with `undefined`. Assignments are not hoisted.In case of `let` and `const` they are also hoisted to the top of their scope but they are not even initialized rather they enter in **Temporal Dead Zone** state.
  - **How does hoisting work with function declarations?**
    >Functions declarations using the `function` keyword are hoisted to the top of their containing scope along with both the function name and its implementation. This allows you to invoke or call e function before it declaration in the code. On the other hand arrow functions hoisting is similar to the default hoisting of `var`, `let` and `const`.
  - **What is the difference between variable declaration and initialization in hoisting?**
    >Declaration refers to the creation of variable using `var`,`let` or `const` and it is hoisted to the top of the scope.Initialization is when a variable is assigned a value and this part is not hoisted.