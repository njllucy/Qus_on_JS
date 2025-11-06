# Qus_on_JS
<b>Qus-1. **Explain the difference between var, let, and const in terms of scope and hoisting. Provide an example where var behaves differently from let and const.**</b><br>

<b> **Answer**</b><br>

**Differences Between var,let And const in terms of scope and hoisting:**<br>

**In scope :**<br>

**var :** var is a function-scoped.Can be Re-declared and can be changed . <br>

can access from outside of a block that's why it is called function scope<br>

**let :** let is a block-scoped.Cannot be Re-declared but can be changed.

 can't access from outside of a block that's why it is called block scope

**const :** const is a block-scoped.Cannot be Re-declared and cannot be changed.

can't access from outside of a block that's why it is called block scope

**In hoisting :**

Hoisting means moving all the variable and functions to the top of their scope before running the code.

**var** : var declarations are hoisted to the top of their scope.

in var if we want to print a variable that is not declared earlier and after the printing line we declare it then this will print undefined  because we are accessing a variable which is not defined earlier.

**let :** let is hoisted, but cannot be accessed before declaration

in var if we want to print a variable that is not declared earlier and after the printing line we declare it then it will just show an reference error 

**const** : Same as let . Hoisted , but cannot be accessed before declaration.<br>
<b>Qus-2. **What is a closure in JavaScript? How does lexical scope enable closures? Provide an example of a closure where an inner function retains access to variables from its outer function.**</b?

<b> **Answer**</b>

**Closure :** Closure is defined as the functions along with it's lexical scope combined together . closures can only  remembers the variables from it’s outer functions scope but not remember it’s own variable and it’s own variable considered to be a local variable.

**Lexical Scope :** Lexical scope means where a variable can be access depend on where it is created not where it is called.Lexical scopes only allows outer varibale not inner one’s.

**How does lexical scope enable closures :**

A function can access variables from the scope in which it was defined, not where it is called.Lexical scope gives the access of the outers variables and closures keeps those accessible variables alive in the memory.The functions knows it’s parent scopes and closures remembers them.<br>
<b>Qus-3. **What is the difference between map(), filter(), and reduce()?**</b>

<b> **Answer**</b>

**map() :** A Map is a collection of key-value pairs.Unlike objects, any type of value can be used as a key

.Keys maintains insertion order.Changes each item in an array and makes a new array.map() transforms the array according to need.

**filter() :**Filters elements based on a condition and returns a new array with only elements that satisfy it.

**reduce() :**Reduces an array to a single value by applying a function.We can also create new arrays, objects, or strings using reduce.

**Differences :** 

map changes each item and returns a new array 

filter picks certain items and returns a new array

reduce combine everything and it returns a single value (can be a number, string, object, or even an array), reduces to one value.<br>

<b>Qus-4. **Explain how JavaScript handles asynchronous operations using Promises and async/await.**</b>

<b> **Answer**</b>

Functions running in parallel with other functions are called asynchronous.

JavaScript normally runs line by line (synchronous).

But sometimes tasks take time.This waiting time freezes our page.To avoid that, JS uses asynchronous programming.Means , JS can start a long task, keep running other code, and finish that task later when ready.

 **Asynchronous operations using Promises and async/await :**

A Promise is an object in JavaScript that represents the  completion (or failure) of an asynchronous task and its resulting value.A Promise represents a value that may be available now, later, or never
Aysnc lets JavaScript do ****tasks that take time without stopping the rest of the program.

Async function always returns a Promise.
Await can only be used inside async functions.
Await pauses execution of the function until the promise resolves.<br>
<b>Qus-5. **How does JavaScript handle type coercion when using == vs. ===? Explain with examples where == results in unexpected behavior due to implicit type conversion.**</b>

<b> **Answer** </b>

In Js Type Coertion happens when Js automatically changes one type of value tanother type

== is known as Equal to &

=== is known as Strict equal to

When we use == in code javascript handle this with auto conversion to a common type before checking equality.

When we use === in code, JavaScript does not handle this with auto conversion to one type, it compares both value and type strictly.

