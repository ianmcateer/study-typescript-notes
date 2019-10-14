apply differently to variables, functions and objects

**Variables:**

type annotations: we(the developer) tell typescript the type of value a variable refers to 

type inference: typescript guesses the type of value a variable refers to

**type annotations:**

```jsx
cd features
mkdir annotations
cd annotations
```

```typescript
const apples: number = 5
```

this type annotiation is trying to tell TS we are only ever going to assign a value of type number to the variable of apples. if ever try to assign another type value will get error

**Primitive Types**

number, boolean, void, undefined, string, symbol, null

**Object types**

functions, arrays, classes, object

```jsx
let apple: number = 5;
let speed: string = 'fast';
let hasName: boolean = true;

// here the value is identiical to its type
let nothingMuch: null = null;

// can only assign it a value of type Date
let now: Date = new Date()
```