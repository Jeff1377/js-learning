# Object

The type value **Object** is used to store any kind of type by keys and more complex entities.
We can create **Object** instance with braces or with **`new`** keyword to an available Class. (see Class section).

```js
const myUser = {
  firstname: 'Gandalf',
  lasntame: 'Leblanc'
};

console.log(myUser); // Object { firstname: "Gandalf", lasntame: "Leblanc" }
```

```js
const myProduct = new Object;
myProduct.price = 300;

console.log(myProduct); // Object { price: 300 }
```

```js
const date = new Date();

console.log(myProduct); // Show instance of Date (with value "now")
```

We access to values with **dot** or **braces**.

```js
const myUser = {
  firstname: 'Gandalf',
  lastname: 'Leblanc'
};

console.log(myUser.firstname); // => Gandalf
console.log(myUser['lastname']); // => Leblanc
```

Any **Object** got default suitable [methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object#instance_properties) and [properties](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object#instance_methods) provided by the language.

The commonly used instance method is **`hasOwnProperty()`**.

```js
const myUser = {
  firstname: 'Gandalf',
  lastname: 'Leblanc'
};

console.log(myUserKeys.hasOwnProperty('firstname')); // => true
```

Or **Object** Class can be used to list in array keys and values, and many other things.

```js
const myUser = {
  firstname: 'Gandalf',
  lastname: 'Leblanc'
};

const myUserKeys = Object.keys(myUser);
const myUserValues = Object.values(myUser);

console.log(myUserKeys); // => Array [ "firstname", "lastname" ]
console.log(myUserValues); // => Array [ "Gandalf", "Leblanc" ]
```

Merge an instance of **Object**:

```js
const myProduct = { name: 'piano' };
const myProductInfo = { name: 'Black piano', price: 200 };

Object.assign(myProduct, myProductInfo);

console.log(myProduct); // => Object { name: "Black piano", price: 200 }

```

## Deleting a property (key)

There isn't any method in an Object itself to delete its own properties (such as Map.prototype.delete()). To do so, one must use the delete operator.

```js
const myUser = {
  firstname: 'Gandalf',
  lastname: 'Leblanc'
};

delete myUser.firstname;

console.log(myUser.firstname); // => undefined
console.log(myUser.firstname); // => Object { lastname: "Leblanc" }
```

---
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object

---