---
title: Javascript
date: 2021-05-03T00:10:22.649Z
---

# [Language](https://gist.github.com/535281fb79c81afcb7af4ecc904ebd07)

## Syntax

<details>

### [The arguments object in JavaScript functions](https://gomakethings.com/the-arguments-object-in-javascript-functions/)

<details>

Within a function, you can use the `arguments` variable to get an array-like list of all of the arguments passed into the function.

You don’t need to define it ahead of time. It’s a native JavaScript object.

</details>

### [Arrow functions in vanilla JS](https://gomakethings.com/arrow-functions-in-vanilla-js/)

<details>

In arrow functions, `arguments` doesn’t exist.

[Rest parameters](https://gomakethings.com/rest-parameters-in-javascript-functions/) do work, however. Here’s the add() function rewritten as an arrow function with rest parameters.

</details>

### [Modern Javascript: Everything you missed over the last 10 years](https://turriate.com/articles/modern-javascript-everything-you-missed-over-10-years) for terminology

</details>

## Closure

### [How Closures Work in JavaScript: A Guide](https://javascript.plainenglish.io/closures-in-javascript-37182198dc20)

<details>

A **closure** is a combination of a function bundled together (enclosed) with references to its surrounding state (the **lexical environment**).

In other words, a closure gives you **access to an outer function’s scope from an inner function**. In JavaScript, closures are created every time a function is created, at function creation time.

#### Disadvantages of Closures

- Closures prevent variables inside functions from being released by memory i.e. as long as the closure is active, the memory can’t be garbage collected. These variables will occupy memory and consume a lot of memory, which may lead to **memory leakage.** The solution to this problem is to delete all unnecessary local variables in time when these variables are not used i.e., set closure to null.

- Creating a function inside a function leads to duplicity in memory and causes the **slowing down of the application**. The solution to this problem is to use closures only when you need privacy. Otherwise, use module patterns to create new objects with shared methods.

</details>

## Patterns

<details>

### [Evolution of Modules in JavaScript with Dependency Injection](https://javascript.plainenglish.io/evolution-of-modules-in-javascript-with-dependency-injection-5c51a3f6442e)

</details>

# State management

<details>

## [Stop using actions in Vuex](https://javascript.plainenglish.io/stop-using-actions-in-vuex-a14e23a7b0e6)

</details>

# Edge

<details>

## [What is FIDO2 WebAuthn? Why you need to seriously consider it for your organization](https://www.secureauth.com/blog/what-is-fido2-webauthn/)

## [New Standards to Access Device Hardware using JavaScript](https://blog.bitsrc.io/new-standards-to-access-user-device-hardware-using-javascript-86b0c156dd3d)

WebHID, WebNFC, and WebUSB have opened up new avenues to interact with user’s device hardware for web apps.

</details>

# 🌟

## 🌟 [JavaScript Execution Context and Hoisting Explained with Code Examples](https://www.freecodecamp.org/news/javascript-execution-context-and-hoisting/)

## 🌟 [The JavaScript `this` Keyword + 5 Key Binding Rules Explained for JS Beginners](https://www.freecodecamp.org/news/javascript-this-keyword-binding-rules/)

## 🌟 [What is the JavaScript Event Loop?](https://javascript.plainenglish.io/what-the-heck-is-event-loop-78ac3c6bde90)

## 🌟 [Don't Confuse Function Expressions and Function Declarations in JavaScript](https://dmitripavlutin.com/javascript-function-expressions-and-declarations/)

# ⭐

## ⭐ [JavaScript setTimeout() – How to Set a Timer in JavaScript or Sleep for N Seconds](https://www.freecodecamp.org/news/javascript-settimeout-how-to-set-a-timer-in-javascript-or-sleep-for-n-seconds/)

<details>

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

</details>

## ⭐ [The Evolution Of Jamstack](https://www.smashingmagazine.com/2021/05/evolution-jamstack/)

## ⭐ [Using Iframes vs Scripts for Embedding Components](https://blog.bitsrc.io/using-iframes-vs-scripts-for-embedding-components-e30eb569cb46)

While Iframes are better with security, rendering than scripts,\
scripts perform better in terms of loading time, SEO, accessibility, responsiveness, etc.

## ⭐️ [The JavaScript Event Propagation: Explained](https://javascript.plainenglish.io/event-propagation-in-javascript-4478852695cf)

<details>

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

</details>

# Visual

## [2D Optics Demos in Javascript](https://www.philipzucker.com/aesthetic-javascript-eduction/)

# Performance

<details>

</details>

# Security

## [7 Steps to Secure JavaScript in 2021](https://blog.bitsrc.io/8-steps-to-secure-javascript-in-2021-6d54d5415264)

<details>

### JavaScript Integrity Checks

```HTML
<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous">
</script>
```

### Frequent Tests for NPM Vulnerabilities

Lately, GitHub introduced a bot name Dependabot, to scan the NPM dependencies automatically and notify you by email stating the risks.

Besides, suppose you enabled the “automated security fix PRs” option. In that case, GitHub will send an automated PR to fix these issues, addressing the security risks in advance.

### Keep Minor and Patch Version Updates Enabled

Have you ever seen ^ or ~ symbol in front of any NPM package version? These symbols indicate the automatic version bump for minor and patch versions.

</details>

# With CSS

## [How to easily add CSS animations to your projects](https://gomakethings.com/how-to-easily-add-css-animations-to-your-projects/)

<details>

For years, my go-to recommendation for CSS animations was [animate.css by Daniel Eden](https://animate.style/).

It’s a great library, but it also _a library_. I generally only need one or two animations, and it includes way more stuff than I typically want in a project.

So I was delighted to discover [Animista by Ana Travis](https://animista.net/) last week. Animista is a tool that lets you select the animation you want, and then copy/paste the CSS for it into your project.

### Important accessibility concerns

Animations can make people who experience motion sickness, vertigo, and other conditions physically sick, dizzy, and disoriented.

Both Windows and macOS provide a way to disable animations at the operating system level, _and_ tell websites that they would prefer not to see them as well.

We can access this setting through a CSS media query: `prefers-reduced-motion`.

```css
@media (prefers-reduced-motion: reduce) {
  /* The user does not want animations */
}

@media (prefers-reduced-motion: no-preference) {
  /* The user is OK with animations */
}
```

</details>

# Reference Code

<details>

## [Snake code golf](https://codepen.io/SleepyPierre/pen/WNpxLZN?editors=0010)

```javascript
const root = document.getElementById("root");
const color = (i, j, c) =>
  (root.children[i].children[j].style.backgroundColor = c);
const isInSnake = (x, y) => s.locs.some((l) => l[0] === x && l[1] === y);
const newS = () => ({
  locs: [[n / 2, n / 2]],
  food: null,
  tdir: 0,
  dir: 0,
  timeout: 0,
});
let n = 20,
  s;
document.onkeydown = ({ keyCode: k }) => {
  if (k === 13) {
    root.innerHTML = Array(n)
      .fill("<div>" + Array(n).fill("<div></div>").join("") + "</div>")
      .join("");
    if (s) clearTimeout(s.timeout);
    s = newS();
    gameLoop();
  }
  if (k > 36 && k < 41 && s.dir % 2 == k % 2) s.tdir = k - 37;
};
const gameLoop = () => {
  document.getElementById("score").textContent = s.locs.length - 1;
  s.dir = s.tdir;
  while (!s.food || isInSnake(...s.food))
    s.food = [0, 0].map(() => Math.floor(Math.random() * n));
  color(...s.food, "#eee");
  const [x, y] = s.locs[0].map((n, i) =>
    s.dir % 2 !== i ? n + s.dir + i - 2 : n
  );
  if ([x, y].every((n, i) => n === s.food[i])) s.food = null;
  else if (Math.min(x, y) < 0 || Math.max(x, y) >= n || isInSnake(x, y)) return;
  else color(...s.locs.pop(), "#333");
  s.locs.unshift([x, y]);
  color(x, y, "#5a7");
  s.timeout = setTimeout(gameLoop, 250);
};
```

</details>

# Link

## [ 고퀄리티⚡개발 컨텐츠 모음](https://github.com/Integerous/goQuality-dev-contents)

## [hacker rank](https://www.hackerrank.com/)
