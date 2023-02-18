# Boolean

Boolean type value is only **true** or **false**.
We use it to store information that will represent an enable or disable state.

```js
let authorizedUser = false;
const isPublishedProduct = true;

console.log(typeof(authorizedUser)) // => 'boolean'
console.log(typeof(isPublishedProduct)) // => 'boolean'
```

This type is also use to create algorytmique logic with **condition** and boolean **operator**.

A given condition need to be **true** or **false** (see: algorythme lesson).

We can set boolean from different way.

```js
const user = {
  name: 'Administrator',
  isAdmin: true
};

const product = {
  name: 'Piano',
  isDeleted: false
}

const authorizeDeleteAction = user && user.isAdmin && !product.isDeleted;

console.log(authorizeDeleteAction); // => true
```

---
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean

---