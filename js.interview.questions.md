# Javascript Interview Questions & Answer

## JavaScript Interview Question Bank

| **Category**                   | **Question**                                                                     | **Answer/Explanation**                                                                                                                                                                                          |
| ------------------------------ | -------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Basics**                     | What are JavaScript primitive data types?                                        | `string`, `number`, `boolean`, `null`, `undefined`, `symbol`, `bigint`.                                                                                                                                         |
|                                | What is the purpose of `typeof`?                                                 | It determines the type of a given value, e.g., `typeof 42 → "number"`.                                                                                                                                          |
|                                | Explain undefined vs not defined.                                                | `undefined`: A variable is declared but not assigned. `not defined`: A variable has not been declared at all.                                                                                                   |
|                                | How does JavaScript handle floating-point arithmetic?                            | Due to binary representation, some calculations may result in precision errors, e.g., `0.1 + 0.2 → 0.30000000000000004`.                                                                                        |
|                                | What is the difference between `==` and `===`?                                   | `==`: Compares values after type coercion; `===`: Compares values without type coercion, e.g., `5 == "5" → true`, `5 === "5" → false`.                                                                          |
| **Scope & Hoisting**           | What is the difference between `let`, `const`, and `var`?                        | `let`: Block-scoped, re-assignable; `const`: Block-scoped, not re-assignable; `var`: Function-scoped, hoisted.                                                                                                  |
|                                | What is hoisting in JavaScript?                                                  | Variables and function declarations are moved to the top of their scope at compile time, e.g., `console.log(a); var a = 5; → undefined`.                                                                        |
|                                | What are closures in JavaScript?                                                 | A closure is a function that retains access to its outer scope, even after the outer function has finished executing. Example: `function outer() { let x = 10; return function inner() { console.log(x); }; }`. |
|                                | What is the Temporal Dead Zone?                                                  | A period in which a variable declared with `let` or `const` is not initialized and trying to access it results in a `ReferenceError`.                                                                           |
| **DOM Manipulation**           | How can you select elements in the DOM?                                          | Using `getElementById`, `querySelector`, `getElementsByClassName`, etc. Example: `document.querySelector(".className")`.                                                                                        |
|                                | What is event delegation?                                                        | A technique where a parent element handles events for its child elements, e.g., adding a single click listener to a parent for multiple child buttons.                                                          |
|                                | What is the difference between `e.preventDefault()` and `e.stopPropagation()`?   | `preventDefault`: Prevents the default browser action (e.g., form submission); `stopPropagation`: Prevents the event from bubbling up the DOM tree.                                                             |
| **Error Handling**             | How does the `try...catch` block work?                                           | `try` block executes code, and if an error occurs, the `catch` block executes. Optionally, a `finally` block executes after `try/catch`.                                                                        |
|                                | What is a promise in JavaScript?                                                 | An object representing a value that will be resolved in the future. It has three states: `pending`, `fulfilled`, `rejected`. Example: `new Promise((resolve, reject) => { resolve('Success'); })`.              |
|                                | What is the difference between `throw` and `return` in error handling?           | `throw`: Exits function execution with an error; `return`: Exits function execution with a value.                                                                                                               |
| **Asynchronous JavaScript**    | What is the Event Loop in JavaScript?                                            | Manages the execution of the main thread, including the call stack, callback queue, and microtasks.                                                                                                             |
|                                | What is the difference between microtasks and macrotasks?                        | Microtasks: Higher priority (e.g., `Promise.then`); Macrotasks: Lower priority (e.g., `setTimeout`). Microtasks execute before macrotasks.                                                                      |
|                                | What are the differences between `setTimeout` and `setInterval`?                 | `setTimeout`: Runs a function once after a delay; `setInterval`: Runs a function repeatedly after a delay.                                                                                                      |
| **Object-Oriented JavaScript** | What is the difference between prototypal inheritance and classical inheritance? | Prototypal inheritance uses objects as prototypes; classical inheritance uses classes. JavaScript is prototypal but introduced class syntax in ES6.                                                             |
|                                | What is the purpose of `Object.create()`?                                        | Creates a new object with the specified prototype object, e.g., `const obj = Object.create(protoObj);`.                                                                                                         |
|                                | Explain the concept of `this` in JavaScript.                                     | `this` refers to the context in which a function is executed. The value of `this` depends on how the function is called.                                                                                        |
| **ES6+ Features**              | What are `let` and `const`?                                                      | `let`: Block-scoped, re-assignable; `const`: Block-scoped, not re-assignable. Both solve issues related to `var`.                                                                                               |
|                                | What is destructuring in JavaScript?                                             | Extracting values from arrays or objects into variables, e.g., `const { name } = obj; const [a, b] = arr;`.                                                                                                     |
|                                | Explain the spread operator (`...`).                                             | Expands elements of an array or object, e.g., `const newArr = [...arr1, ...arr2]; const newObj = { ...obj1, ...obj2 };`.                                                                                        |
| **Data Structures**            | What are `Maps` and `Sets` in JavaScript?                                        | `Map`: Key-value pairs with any key type; `Set`: Unique values collection.                                                                                                                                      |
|                                | What is the difference between `Array` and `Set`?                                | `Array`: Allows duplicate values, indexed; `Set`: Only unique values, unordered.                                                                                                                                |
|                                | How does the `reduce` method work?                                               | Applies a callback to each element, accumulating a single result, e.g., `[1, 2, 3].reduce((acc, curr) => acc + curr, 0) → 6`.                                                                                   |
| **Modules**                    | What is the difference between `default` and `named exports`?                    | `default`: Only one per file, imported without curly braces; `named`: Multiple per file, imported with curly braces.                                                                                            |
|                                | What is `import` and `export` in JavaScript?                                     | `import` loads modules, `export` defines what a module exposes, e.g., `export const x = 5; import { x } from './module.js';`.                                                                                   |
| **Web APIs**                   | What is the difference between `fetch` and `XMLHttpRequest`?                     | `fetch` is promise-based and simpler; `XMLHttpRequest` uses callbacks and has more complexity.                                                                                                                  |
|                                | How does `CORS` work in JavaScript?                                              | Cross-Origin Resource Sharing (CORS) allows restricted resources from another origin. Managed via HTTP headers.                                                                                                 |
| **Miscellaneous**              | What is the difference between synchronous and asynchronous code?                | Synchronous: Executes sequentially; Asynchronous: Executes non-blocking operations, like using callbacks or promises.                                                                                           |
|                                | What are `polyfills`?                                                            | Code added to provide modern features in older browsers, e.g., adding Promise support to IE11.                                                                                                                  |

## Common JavaScript Questions and Answers

| **Question**                                            | **Answer**                                                                                              |
| ------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- |
| What is `undefined` and `null` in JavaScript?           | `undefined`: A variable is declared but not assigned a value. `null`: Explicitly represents "no value". |
| What is `NaN` in JavaScript?                            | `NaN` stands for "Not a Number". It is a result of invalid arithmetic operations (e.g., `0/0`).         |
| What will `typeof null` return?                         | `"object"` (a historical bug in JavaScript).                                                            |
| What are falsy values in JavaScript?                    | `0`, `false`, `""` (empty string), `null`, `undefined`, and `NaN`.                                      |
| What will `[] == false` return?                         | `true` because the array is coerced to an empty string (`""`), and `"" == false`.                       |
| What is hoisting in JavaScript?                         | Variable and function declarations are moved to the top of their scope before code execution.           |
| What will `typeof NaN` return?                          | `"number"` because `NaN` is considered a numeric type.                                                  |
| What is the difference between `map()` and `forEach()`? | `map()`: Returns a new array. `forEach()`: Executes a function for each element, no return.             |

## Most Popular Coding Challenges

| **Category**   | **Question**                                 | **Solution Overview**                                                                                    |
| -------------- | -------------------------------------------- | -------------------------------------------------------------------------------------------------------- |
| **Strings**    | Reverse a string.                            | Use `split`, `reverse`, and `join`. Example: `'hello'.split('').reverse().join('')` → `'olleh'`.         |
|                | Check if a string is a palindrome.           | Compare the string with its reverse. Example: `'racecar' === 'racecar'.split('').reverse().join('')`.    |
| **Arrays**     | Find the maximum value in an array.          | Use `Math.max` with the spread operator: `Math.max(...arr)`.                                             |
|                | Remove duplicates from an array.             | Use `Set`: `[...new Set(arr)]`.                                                                          |
| **Objects**    | Deep clone an object.                        | Use `structuredClone` or `JSON.parse(JSON.stringify(obj))`.                                              |
| **Algorithms** | Implement the Fibonacci sequence.            | Use recursion or iteration. Example: `function fib(n) { return n <= 1 ? n : fib(n - 1) + fib(n - 2); }`. |
| **Sorting**    | Sort an array of numbers in ascending order. | Use `.sort((a, b) => a - b)`.                                                                            |

## Scenarios and Examples of Type Coercion

| **Scenario**                                        | **Example**                                  | **Explanation**                                                                                     |
| --------------------------------------------------- | -------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| **Number + String → String Concatenation**          | `5 + "10" → "510"`                           | The number `5` is coerced into a string and concatenated with `"10"`.                               |
| **Boolean → Number**                                | `true + 1 → 2`, `false + 1 → 1`              | `true` is coerced to `1` and `false` to `0`.                                                        |
| **String → Number**                                 | `"5" - 2 → 3`, `"5" * 2 → 10`                | JavaScript converts the string `"5"` into a number for arithmetic operations.                       |
| **Null → Number**                                   | `null + 5 → 5`                               | `null` is coerced to `0`.                                                                           |
| **Undefined → Number**                              | `undefined + 5 → NaN`                        | `undefined` cannot be converted into a number and results in `NaN`.                                 |
| **Array → String**                                  | `[1, 2] + "" → "1,2"`                        | Arrays are coerced to strings by calling `.toString()`.                                             |
| **Object → String or Number**                       | `{} + "" → "[object Object]"`                | Objects are coerced to their string representation, calling `.toString()` by default.               |
| **Array + Number → String Concatenation**           | `[1, 2] + 3 → "1,23"`                        | The array is coerced into a string, then concatenated with `3`.                                     |
| **Implicit Boolean Coercion in Logical Operations** | `!!"hello" → true`, `!!0 → false`            | Non-empty strings are `true`, `0` is `false`. `!!` explicitly coerces to a boolean.                 |
| **Falsy Values in JavaScript**                      | `0, null, undefined, "", NaN`                | All these values are treated as `false` in a boolean context. Example: `if (0)` → does not execute. |
| **String Coercion with Template Literals**          | `` `Value is ${5}` → "Value is 5" ``         | Template literals implicitly convert non-string values to strings.                                  |
| **Equality Comparisons (== vs ===)**                | `5 == "5" → true`, `5 === "5" → false`       | `==` performs type coercion. `===` checks strict equality without coercion.                         |
| **Combining Arrays and Objects in Strings**         | `[] + {} → "[object Object]"`, `{} + [] → 0` | Array coerces to `""`, and object to `"[object Object]"`. The order of operations matters.          |

## Explicit Coercion

| **Operation**                    | **Example**                           | **Explanation**                                                                                  |
| -------------------------------- | ------------------------------------- | ------------------------------------------------------------------------------------------------ |
| **String → Number**              | `Number("42") → 42`                   | Converts a string into a number explicitly.                                                      |
| **Boolean → Number**             | `Number(true) → 1`                    | `true` converts to `1`, and `false` to `0`.                                                      |
| **Number → String**              | `String(42) → "42"`                   | Converts a number into a string explicitly.                                                      |
| **String → Boolean**             | `Boolean("hello") → true`             | Non-empty strings are `true`.                                                                    |
| **Number → Boolean**             | `Boolean(0) → false`                  | Zero is `false`, non-zero numbers are `true`.                                                    |
| **Parsing Numbers from Strings** | `parseInt("10px") → 10`               | Extracts integers from strings.                                                                  |
| **Forcing Conversion to Number** | `+"42" → 42`                          | The unary `+` operator converts a string into a number.                                          |
| **Object → Primitive**           | `({}).toString() → "[object Object]"` | Converts objects into their primitive string representation using `.toString()` or `.valueOf()`. |

## Common Interview Questions on Type Coercion

| **Question**                                                            | **Answer/Explanation**                                                                                                      |
| ----------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| **What happens when you compare null with undefined using ==?**         | `null == undefined → true`, because they are loosely equal.                                                                 |
| **Why does "5" - 2 return 3, but "5" + 2 returns "52"?**                | `"-"` triggers numeric conversion, `"+"` triggers string concatenation.                                                     |
| **What are "truthy" and "falsy" values in JavaScript?**                 | **Truthy**: Non-empty strings, numbers except 0, non-null objects. **Falsy**: 0, `""`, `null`, `undefined`, `NaN`, `false`. |
| **Why does {} + [] return 0 but [] + {} return "[object Object]"?**     | Depends on the order of evaluation and coercion rules. `{}` is treated as a code block in the first case.                   |
| **What is NaN === NaN?**                                                | `false`, because `NaN` is not equal to anything, including itself.                                                          |
| **How can you explicitly check if a value is NaN?**                     | Use `Number.isNaN(value)` or `isNaN(value)`.                                                                                |
| **What is the result of null + 5?**                                     | `5`, because `null` is coerced to `0`.                                                                                      |
| **What is the difference between parseInt("10px") and Number("10px")?** | `parseInt("10px") → 10` (parses valid leading numbers). `Number("10px") → NaN` (fails for non-numeric characters).          |
| **What is [] == ![] in JavaScript?**                                    | `true`, because `![]` is `false`, and `[] == false` triggers coercion where `[]` becomes an empty string (`""`).            |

## JavaScript Type Coercion Cases (with examples)

| **Expression**       | **Result**                 | **Explanation**                                                                               |
| -------------------- | -------------------------- | --------------------------------------------------------------------------------------------- |
| `5 + "10"`           | `"510"`                    | Number (`5`) is coerced to string and concatenated with `"10"`.                               |
| `5 + true`           | `6`                        | `true` is coerced to `1`, so `5 + 1 = 6`.                                                     |
| `5 + false`          | `5`                        | `false` is coerced to `0`, so `5 + 0 = 5`.                                                    |
| `"5" - 3`            | `2`                        | String (`"5"`) is coerced to number and subtraction occurs.                                   |
| `"5" * "2"`          | `10`                       | Both strings are coerced to numbers for multiplication.                                       |
| `"5" / "2"`          | `2.5`                      | Both strings are coerced to numbers for division.                                             |
| `"5" - true`         | `4`                        | `"5"` is coerced to `5`, `true` is coerced to `1`, so `5 - 1 = 4`.                            |
| `"5" + null`         | `"5null"`                  | `null` is coerced to string `"null"`, and concatenated.                                       |
| `"5" * null`         | `0`                        | `null` is coerced to `0`, so multiplication results in `0`.                                   |
| `5 + undefined`      | `NaN`                      | `undefined` cannot be coerced to a number, resulting in `NaN`.                                |
| `5 == "5"`           | `true`                     | Loose equality (`==`) coerces `"5"` to a number.                                              |
| `5 === "5"`          | `false`                    | Strict equality (`===`) does not perform type coercion, so types mismatch.                    |
| `null == undefined`  | `true`                     | Special case: `null` and `undefined` are loosely equal.                                       |
| `null === undefined` | `false`                    | Strict equality requires type and value to be the same, which they are not.                   |
| `!!"text"`           | `true`                     | Non-empty strings are truthy.                                                                 |
| `!!""`               | `false`                    | Empty strings are falsy.                                                                      |
| `!!0`                | `false`                    | Zero is falsy.                                                                                |
| `!!1`                | `true`                     | Non-zero numbers are truthy.                                                                  |
| `[] + {}`            | `"[object Object]"`        | The array is coerced to an empty string and object to its string representation.              |
| `{}` + `[]`          | `0` or `"[object Object]"` | Behavior depends on the engine (interpreted differently in browsers like Chrome vs. Node.js). |
