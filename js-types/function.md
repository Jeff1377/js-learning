## Function

Like other type of values, a **function** can be store in a **variable**, in **object property**, in an **array item**, they will got type **function**

A function can be declare with a modern way (since ES6)

```js
const doThat = () => {};

console.log(typeof(doThat)); // 'function'
```

Or function can be declare with a classic way

```js
function doThat() {}

console.log(typeof(doThat)); // 'function'
```

A function can receive one ore several **parameters** / **attributes**, and can be use like variable only in scope of braces.

```js
function logMyUser(firstname, lastname) {
  console.log('My user is ' + firstname + ' ' + lastname);
}

logMyUser('Gandalf', 'Leblanc'); // => 'My user is Gandalf Leblanc'
```

A **function** can return value.

With **braces** you need to use the word **return**.

```js
const getPercentage = (quantity, total) => {
  return (100 / total) * quantity;
}

const totalPeople = 30;
const totalGirls = 6;

const girlPourcentage = getPercentage(totalGirl, totalPeople);

console.log(girlsPourcentage); // => 20

```

If your function need to return a result from one instruction, you can declare without braces and without the word **return** (only in modern way).

```js
const getPercentage = (quantity, total) => (100 / total) * quantity;

const totalPeople = 30;
const totalGirls = 6;

const girlPourcentage = getPercentage(totalGirl, totalPeople);

console.log(girlsPourcentage); // => 20

```

---
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function

---