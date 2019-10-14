```typescript
// Array of strings
// type array that contains strings
let colors: string[] = ['red','green','blue'];
let myNumbers: number[]= [ 1, 2, 3];
let truths: boolean[] = [true, true, false];

// Classes
class Car {
    
}

// capital means refering type of class Car
// the variable car is only ever going to refer to an instance of Car
let car: Car = new Car()

// Object literal
let point = {
    x: 10,
    y: 20,
}
// declaring variable point assinging an object and adding type annotation 
let point: { x: number; y: number} = {
    x: 10,
    y: 20,
}



```