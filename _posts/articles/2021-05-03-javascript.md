---
title: Javascript
date: 2021-05-03T00:10:22.649Z
---

# 🌟

## [JavaScript Execution Context and Hoisting Explained with Code Examples](https://www.freecodecamp.org/news/javascript-execution-context-and-hoisting/)

## [The JavaScript `this` Keyword + 5 Key Binding Rules Explained for JS Beginners](https://www.freecodecamp.org/news/javascript-this-keyword-binding-rules/)

## [What is the JavaScript Event Loop?](https://javascript.plainenglish.io/what-the-heck-is-event-loop-78ac3c6bde90)

## [Don't Confuse Function Expressions and Function Declarations in JavaScript](https://dmitripavlutin.com/javascript-function-expressions-and-declarations/)

# ⭐

## [JavaScript setTimeout() – How to Set a Timer in JavaScript or Sleep for N Seconds](https://www.freecodecamp.org/news/javascript-settimeout-how-to-set-a-timer-in-javascript-or-sleep-for-n-seconds/)

setTimeout() method syntax

```javascript
setTimeout(function, milliseconds, parameter1, parameter2, ...);
```

setTimeout() with additional parameters for the function

```javascript
function greeting(name, role) {
  console.log(`Hello, my name is ${name}`);
  console.log(`I'm a ${role}`);
}

setTimeout(greeting, 3000, "Nathan", "Software developer");
```

Now you may be thinking, "why not just pass the parameters directly to the function?"

This is because if you pass the parameters directly like this:

```javascript
setTimeout(greeting("Nathan", "Software developer"), 3000);
```

Then JavaScript will immediately execute the function without waiting, because you're passing a function call and not a function reference as the first parameter.

# Tool

## [Pts](https://github.com/williamngan/pts)

Pts is a typescript/javascript library for visualization and creative-coding.
