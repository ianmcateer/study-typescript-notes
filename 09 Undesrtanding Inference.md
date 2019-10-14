can rmeove all previous type annotations and still not get any errors- some TS then infers the type

**Type Inference**

```jsx
const color = 'red';
```

the first part const color is variable declaration

the second step is variable initialisaiton

**if we do declaraiton and initialisation are on the same line ts will figure out the type of ‘color’ for us **

if move assignment to a different line it wont work anymore

**why use one over the other?**

we will rely on type inference all the time wherever we can