we will rely on type inference heavily, but some scearios we want to use type declaration

first example is funciton that returns the any type

```jsx
// when to sue annotations
// 1 function that returns any type

const json = '{"x": 10, "y": 20}'
const output = JSON.parse(json)
console.log(output)


// problem with any is this..
// ts doesnt throw error here 
output.fhsfhdshfdskf
```

right now ts this output is of type: any

```jsx
'false' once we parse get back a boolean
'4' once we parse it get back a number
```

we can clearly pass in very different strings into this funciton and get back very different types- TS cannot predict these differnt types bc it depends onthe string we put into the funciton

the any type means TS has no idea what value is being returned from JSON.parse()

**type: any**

**
**

- a type jsut as ‘string’ and ‘boolean’ are

- means TS has no idea what this is

**- avoid variables with ‘any’ at all costs**