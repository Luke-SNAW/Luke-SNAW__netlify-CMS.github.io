---
title: Javascript
date: 2021-05-03T00:10:22.649Z
---

# 🌟

## 🌟 [JavaScript Execution Context and Hoisting Explained with Code Examples](https://www.freecodecamp.org/news/javascript-execution-context-and-hoisting/)

## 🌟 [The JavaScript `this` Keyword + 5 Key Binding Rules Explained for JS Beginners](https://www.freecodecamp.org/news/javascript-this-keyword-binding-rules/)

## 🌟 [What is the JavaScript Event Loop?](https://javascript.plainenglish.io/what-the-heck-is-event-loop-78ac3c6bde90)

## 🌟 [Don't Confuse Function Expressions and Function Declarations in JavaScript](https://dmitripavlutin.com/javascript-function-expressions-and-declarations/)

# ⭐

## ⭐ [JavaScript setTimeout() – How to Set a Timer in JavaScript or Sleep for N Seconds](https://www.freecodecamp.org/news/javascript-settimeout-how-to-set-a-timer-in-javascript-or-sleep-for-n-seconds/)

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

## ⭐ [The Evolution Of Jamstack](https://www.smashingmagazine.com/2021/05/evolution-jamstack/)

## ⭐ [Using Iframes vs Scripts for Embedding Components](https://blog.bitsrc.io/using-iframes-vs-scripts-for-embedding-components-e30eb569cb46)

While Iframes are better with security, rendering than scripts,\
scripts perform better in terms of loading time, SEO, accessibility, responsiveness, etc.

## ⭐️ [The JavaScript Event Propagation: Explained](https://javascript.plainenglish.io/event-propagation-in-javascript-4478852695cf)

### Event Delegation

- Event delegation is the technique of handling events on our web page in a better way. Event delegation is **based upon event bubbling.** So just because **event bubbling exists, event delegation also exists.**
- On our web page we have a number of events, and as an application grows events also keep on increasing. At some point in time, we have a lot of event handlers just hanging around on our web page, which is a critical performance bottleneck. So that is why we use event delegation.
- Suppose in e-commerce sites we have a lot of categories, like laptops, shoes, fashion, etc. So whenever we click on a laptop it takes to laptops and so on. Generally, we attach event listeners to each category. And that is not a good way to do it, we can have infinite categories.
- A better way to handle this is, instead of attaching event handlers to each and every child element or HTML element individually, we should rather attach event handlers to the parent of these elements.
- **Single event handler to parent.** Then on click of the child element, events will bubble out to their parents. The parent is listening to all the events happening in the child elements.

### Accessing Propagation Information

- **e.target** references the event target.
- **e.currentTarget** is the node on which the running listener was registered on. This is the same value of the listener invocation context, i.e, the value referenced by the `this` keyword.
- We can even find out the current phase with **e.eventPhase**. It is an integer that refers to one of the three `Event` constructor constants `CAPTURING_PHASE`, `BUBBLING_PHASE` and `AT_TARGET`.

### Stopping Immediate Propagation

### Event Cancellation

Some events are associated with a **default action that the browser executes at the end of the propagation**. For instance, the click on a link element or the click on a form submit button causes the browser to navigate to a new page, or submit the form respectively.

It is possible to avoid the execution of such default actions with the event cancellation, by calling yet another method of the event object, **e.preventDefault**, in a listener. But this method does not stop the event from bubbling up the DOM.

However, there is one more way to **return false**. It prevents the browser's default behavior, prevents the event from bubbling up the DOM, and immediately returns from any callback.

```
return false = e.preventDefault + stopPropagation + (stops callback execution)
```




# Tool

## [Pts](https://github.com/williamngan/pts)

Pts is a typescript/javascript library for visualization and creative-coding.

# Link

## [{ 고퀄리티⚡개발 컨텐츠 모음 }](https://github.com/Integerous/goQuality-dev-contents)

## [hacker rank](https://www.hackerrank.com/)