# Javascript Type

The **types** give us information of our values nature.

## Store values with variable
3 ways to create / instance / declare a **JS** variable

---
### Historic way (Before the advent of ES6)
* **var** => Nice and innocent way to declare a variable

### Modern ways
* **let** => value can change
* **const** => value can't change


```js
var myVar = '';
myVar = 'ok';

console.log(myVar); // => 'ok'
```

```js
let myLet = '';
myLet = 'ok';

console.log(myLet); // => 'ok'
```

```js
const myConst = '';
myConst = 'ok';

Uncaught TypeError: invalid assignment to const 'test'
```

## IMPORTANT
A const value can't be reassigned (=) **but** an array or an object from a constant can change any items, properties

```js
const myConstWithArray = ['A', 'B', 'D'];
myConstWithArray[2] = 'C';

console.log(myConstWithArray); // => ['A', 'B', 'C']

myConstWithArray.push('D');
console.log(myConstWithArray); // => ['A', 'B', 'C', 'D']

myConstWithArray.shift();
console.log(myConstWithArray); // => ['B', 'C', 'D']
```
```js
const myConstWithObject = {film: 'Gosth', animal: 'piano'};
myConstWithObject.animal = 'cat';

console.log(myConstWithObject); // => {film: 'Gosth', animal: 'cat'}
```

---
https://www.freecodecamp.org/news/var-let-and-const-whats-the-difference/

---


## other way to store value

### In object

```js
const user = {firstname: 'Gandalf', lastname: 'Leblanc', age: 1432};
```

### In array

```js
const fruits = ['banana', 'apple'];
```

# Possible types of values

* **[number](https://github.com/Jeff1377/js-learning/tree/main/js-types/number.md)** (integer, int)
* **[string](https://github.com/Jeff1377/js-learning/tree/main/js-types/string.md)**
* **[boolean](https://github.com/Jeff1377/js-learning/tree/main/js-types/boolean.md)** (bool)
* **[undefined](https://github.com/Jeff1377/js-learning/tree/main/js-types/undefined.md)**
* **[null](https://github.com/Jeff1377/js-learning/tree/main/js-types/null.md)**
* **nullN**
* **functionnull(method)
* **array** (iterator, list)
* **object** (hash)

---