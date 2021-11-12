Async Programming is JS
=======================

Callbacks
---------

Callbacks are the original and most basic way to handle async programming in JS.

> A callback function is a function passed into another function as an argument, which is then invoked inside the outer function to complete some kind of routine or action.

[MDN](https://developer.mozilla.org/en-US/docs/Glossary/Callback_function)

---

```js
function done() {
  document.write('Done')
}

function wait(callback) {
  setTimeout(callback, 1000)
}

wait(done)
window.addEventListener('load', () => {
  document.write('Starting...')
})
```

Callback issues
---------------

- Can lead to deeply nested code blocks
- Lacks error handling

Promise
-------

> The Promise object represents the eventual completion (or failure) of an asynchronous operation and its resulting value.

[MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)

States
------

A Promise is in one of these states:

- Pending - initial state, neither fulfilled nor rejected
- Fulfilled - meaning that the operation was completed successfully
- Rejected - meaning that the operation failed

Prototype Methods
-----------------

- .then() - Appends fulfillment handlers (and optionally rejection handlers)
- .catch() - Appends rejections handlers

Methods
-------

- .resolve(value) - Returns a new `Promise` resolved to the supplied `value`
- .reject(reason) - Returns a new `Promise` rejected with the given `reason`

---

```js
function write(msg) {
  document.write(msg)
}

const wait = new Promise((resolve, reject) => {
  setTimeout(() => {
    resolve('Done')
  }, 1000)
})

wait.then(write)
window.addEventListener('load', () => {
  document.write('Starting...')
})
```

Await
-----

> The await operator is used to wait for a Promise. It can only be used inside an async function within regular JavaScript code; however it can be used on its own with JavaScript modules.

[MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/await)

---

```js
function write(msg) {
  document.write(msg)
}

const wait = new Promise((resolve, reject) => {
  setTimeout(() => {
    resolve('Done')
  }, 1000)
})

const message = await wait
write(message)
```

async
-----

> An async function is a function declared with the async keyword, and the await keyword is permitted within them. The async and await keywords enable asynchronous, promise-based behavior to be written in a cleaner style, avoiding the need to explicitly configure promise chains.

[MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/async_function)

---

`async` allows implicit `Promise` creation

```js
async function foo() {
   return 1
}
```

is similar to

```js
function foo() {
   return Promise.resolve(1)
}
```
