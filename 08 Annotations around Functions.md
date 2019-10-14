```typescript
// Function type annotation
const logNumber = (i: number) => {
    console.log(i)
}

// how do we add type annotation for this function?
// rememebr type annotation to descrivbe what type of a value we want to assing to that variable
const logNumber = (i: number) => {
    console.log(i)
}
```

as a funciton we care about what arguments going into function and what values the function should return

```typescript
const logNumber: (i: number) => void = (i: number) => {
    console.log(i)
}
```

looks nasty syntax