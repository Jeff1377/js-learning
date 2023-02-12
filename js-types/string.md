## String

To store any kind of text we use string type.

We can create string with simple quote (**'**), double quote (**"**) or back quote (**`**)

```js
const title = 'My Page';
const description = "My description";
const label = `My label`

console.log(title, description, label); // 'My Page My description My..'
console.log(typeof(title)); // 'string'
```

### String interpolation

We can interpolate **string** (and **number**) with operator addition (**+**)

```js
const userLastName = 'Le Blanc';
const userFirstName = 'Gandalf';
const helloText = 'Bonjour ' + userFirstName  + ' ' + userLastName;

console.log(helloText); // => 'Bonjour Gandalf Le Blanc'
```

An other way to do interpolation is possible with back quote (**`**)
```js
const userLastName = 'Le Blanc';
const userFirstName = 'Gandalf';
const helloText = `Bonjour ${userFirstName} ${userLastName}`;

console.log(helloText); // => 'Bonjour Gandalf Le Blanc'
```

---
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String

---