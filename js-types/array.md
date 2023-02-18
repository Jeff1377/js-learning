# Array

The type value **Array** is an element that can store a list of items (values/elements) with any kind of type.


```js
const myArrayOfNumber = [1, 2, 3];
const myArrayOfString = ['A', 'B', 'C'];

const myArrayOfAnything = [
  1,
  'A',
  true,
  ['An other Array', ['An other array within other Array' ]],
  { or: 'An object', withinOtherArray: [1, 2, 3, ['An another Array'] ] },
  null,
  undefined,
  (callMeAtSeven) => ['I am a string in returned array'] },
  function(callMeAtHeight) { return ['I am a string in returned array']; },
  new Date(),
]
```

In JS, an **Array** is not primitive, like an object he got suitable methods and properties provided by the language.

We create **Array** with bracket or new instance of **Array**

```js
const emtpyArrayFromBracket = [];

const filledArrayFromNew = new Array(1, 2, 3);

console.log(emtpyArrayFromBracket) // => Array(0) [ ]
console.log(filledArrayFromNew) // => Array(3) [ 1, 2, 3 ]
```

That why the method **typeof(anArray)** will return 'object'.

### Property example

```js
// The length property contains the number of items
const items = ['A', 'B', 'C'];

items.lenght // => 3

typeof(items) // => 'object'
```

### Method example

```js
// The foreach method is use to iterate on each item (item receive by given method in first attribute).
const items = [1, 2, 3];

items.forEach((item) => { console.log(item); });
```

## Access to items (values, elements)

To access to any item of **Array** you have to use an number (integer).

But given string of number are allowed...

The first item start from **index** (range): **0**.

```js
const items = ['A', 'B', 'C'];

console.log(items[0]) // => "A"
console.log(items[1]) // => "B"
console.log(items[2]) // => "C"

console.log(items['2']) // => "C"

console.log(items.0); // A syntax error
```

We can add properties or methods in an **Array**.

Not to be confused: Properties and methods are not included in the items list

### Property example

```js
const items = ['A', 'B', 'C'];

items.myProperty = 'I am property';

console.log(items.myProperty);    // => 'I property'
console.log(items['yPropmyPropertyerty']); // => 'I property'

console.log(items); // => Array(3) [ "A", "B", "C" ]
```

### Method example

```js
items['myMethod'] = () => 'I am an method';

console.log( items.myMethod() );    // => 'I am an ugly method'
console.log( items['myMethod']() ); // => 'I am an ugly method'

console.log(items); // => Array(3) [ "A", "B", "C" ]
```

---
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array

---