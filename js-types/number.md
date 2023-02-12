## Number
In **JS** a **number** can be integer, short, long, float...
Isn't case for some other languages

```js
const myInteger = 1;
typeof(myInteger); // => 'number'
```
```js
const myFloat = 1.05;
typeof(myFloat); // => 'number'
```
```js
const fakeNumber = '15';
typeof(fakeNumber); // => 'string'
```

We use number to store any kind of data.
* user **age**
* product **price**
* element position **x, y, z**
* longitude / latitude
* ...


Numbers can be used to do operations (with **operator**), count something (**counter**), find an item in an array (**index**/**range**) or many other thing needed by our script.

```js
const productPrice = 30;
const totalSelectedProducts = 2;

const totalPrice = productPrice * totalSelectedProducts;

console.log(totalPrice); // => 60
```

```js
const fruits = ['apple', 'orange', 'banana']
const itemIndex = 2;

console.log(letterArray[itemIndex]); // => 'banana'
```

Its authorized to use operator addition (**+**) between number type and string type to do **interpolation**.

```js
const minimumAgeAuthorized = 18;

const minAgeText = 'You must be ' + minimumAgeAuthorized + ' to enter';

console.log(minAgeText); // => 'you must be 18 to enter'
```

But other operation will respond **NaN**

```js
const anyNumber = 4;

anyNumber * 'a'; // => NaN
anyNumber / 'a'; // => NaN
anyNumber - 'a'; // => NaN

const badOperation = 'a' * [];
console.log(badOperation) // => NaN

const OMG = 3 + NaN; // => NaN
```

**JS** ensure a max safe integer:
* **9007199254740991**
* **-9007199254740991**

But some browser can got more bigger: **99999999999999999999**

If number is too big **JS** will transform it with an exposant (**squared**)

```js
const bigNumber = 999999999999999999999;

console.log(bigNumber); // => 1e+21
```

---
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number

---