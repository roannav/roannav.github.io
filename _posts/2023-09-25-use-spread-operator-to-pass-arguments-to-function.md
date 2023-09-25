---
layout: default
title: Use Spread Operator to Pass an Argument in JavaScript 
---

# Using the Spread Operator to Pass Arguments to a Function in JavaScript

Also read: [3 simple use cases for the spread operator](2023-09-24-JavaScript-spread-operator.md)


## Quick Way to Pass ARRAY ELEMENTS to a Function

```
const names = ["Art", "Bill", "Cleo"];

function storyLine( person1, person2, person3) {
  console.log(`${person1} is friends with ${person2} and ${person3}.`);
}

// The storyLine() function is expecting
// 3 arguments, so we can pass the values
// in array names, by using the spread operator.
storyLine(...names);
```

## WARNING: Don't Pass OBJECT PROPERTIES this way though

```
const object1 = {
  firstName: "Maria",
  lastName: "Zawadi",
  age: 32
}

function storyLine2( firstName, lastName, age) {
  console.log(`${firstName} ${lastName} is ${age} years old.`);
}

// hidden bug
storyLine2(...Object.values(object1));
```

Though this may appear to work, it won't always.
Because the order of the object properties is not
guaranteed, you might be passing, for example, `32` as the first argument.

# Solution

One way to fix this situation is to modify the function's parameter declarations by destructuring the object.

```
function storyLine3({firstName, lastName, age}) {
  console.log(`${firstName} ${lastName} is ${age} years old.`);
}

storyLine3(object1);
```

NOTE: This technique is often used to pass props to React components.

# Compare Invoking a Function With or Without Object Destructuring 

Long way (without object destructuring):

`storyLine2(object1.firstName, object1.lastName, object1.age);`

Better (with object destructuring):

`storyLine3(object1);`