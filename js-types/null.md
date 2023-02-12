## Null

The null value is not undefined, not false, not empty.

He represents the intentional absence of any object value.

```js
let userLevel = null;

console.log(typeof(userLevel)); // => 'object' (not "null" for legacy reasons)
```

It is one of JavaScript's primitive values and is treated as falsy for boolean operations.

```js
let favoriteCoffee = null;

if (!favoriteCoffee) {
  favoriteCoffee = 'Malongo';
}

console.log(favoriteCoffee)// => Malongo
```

Difference between null and undefined

```js
null === undefined; // false
null == undefined; // true
null === null; // true
null == null; // true
!null; // true
1 + null; // false
1 + undefined; // NaN
```

---
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/null

---