**Type:**

string: “hi there”

number: 0.003, 40

boolean: true

Date: new Date()

Todo: {id: 1, competed: false}

primitive types: numebr, string, boolean, void, undefined, symbol, null

object types: functions, classes, arrays, objects, any types we create ourselves

we can trick ts compiler in a good way with object types

**why care about types? **

types are used by the compielr to analyse our code for errors

types allow other engineers to understand what values are flowing around our codebase

### Examples of Types

```jsx
mkdir features
touch types.ts
```

every value(everything we assign to a variable) has a type

```jsx
const today = new Date();
```

ts knows what properties a date has thats why they show up as suggestion

Types: here are the properties and methods that this value has

```jsx
const person = {
    age: 20
}

class Color {
    
}
const red = new Color ();
```

if hover over red ts knwos this variable points to an object that is of type Color

### Where do we use types?

Everywhere! - every value inside system has a type

**a type is a shortcut to refer to the different properties and functions that a value has **

**any value has a type **

**we care about types bc they give the ts compiler information to analyse our code for errors **

