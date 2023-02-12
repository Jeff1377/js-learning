## Undefined

The "non value" **undefined** is given to a variable or attribute not set yet.

Declare variable without setting value (**=**), his value will be **undefined**.

```js
const myValueUndefined;

console.log(myValueUndefined); // => undefined
console.log(typeof(myValueUndefined)); // => undefined
```

**Dont mix up**: if you want use a variable who dont exist yet. (its an error!).

```js
console.log(notExistingVariable);

Uncaught ReferenceError: notExistingVariable is not defined
```

You will got **undefined** type if you ask an **object** property or an **array** item

```js
const user = {
  name: 'Merlin'
}

console.log(user.birthday); // => undefined

const fruits = ['apple', 'banana'];

console.log(fruits[999]); // => undefined
```

A **function** without **return** word will return **undefined**.

```js
const doSomething = () => {};

const result = myFunction();

console.log(result); // => undefined
```

---
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Undefined

---