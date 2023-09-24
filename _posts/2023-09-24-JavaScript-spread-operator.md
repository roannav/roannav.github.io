# The Spread Operator in JavaScript

`...` was a new feature in ES6.

The spread operator lets you spread all the elements of an array, object or string.

# 3 Use Cases

## Concat Arrays
```
const array1 = ['a', 'b', 'c'];
const array2 = ['c', 'd'];

const combinedArray = [...array1, ...array2];
console.log(combinedArray);
```

Result:

`[ 'a', 'b', 'c', 'c', 'd' ]`

Note:  there was the same element `'c'` in both input arrays.
The combined array will have 2 of these `'c'` elements.


## Combining Objects
```
const object1 = {
  firstName: "Maria",
  lastName: "Adams"
}
const object2 = {
  lastName: "Zawadi",
  age: 32
}

const combinedObject = { ...object1, ...object2 };
console.log(combinedObject);
```

Result:
```
{
  firstName: 'Maria',
  lastName: 'Zawadi',
  age: 32
}
```

Note: both objects had the same property `lastName`.
For that property, the 2nd object overwrote the 1st object.

In the case of arrays, the element that was in both input arrays,
became **duplicated** in the combined array.
However, in the case of objects, you can't just list the property
twice with 2 different values.  So instead the property is **overwritten**,
by the 2nd object.


## Split String into Chars
```
const str = "rabbit";

const chars = [...str];
console.log(chars);
```

Result:

`[ 'r', 'a', 'b', 'b', 'i', 't' ]`
