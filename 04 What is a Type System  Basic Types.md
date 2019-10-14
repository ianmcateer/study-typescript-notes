quick overview of course: 

two catageories of knowledge

1- syntax and features: what is an interface, what is the syntax for defining and interface

2- design patterns with TS- how do we use interfaces to write reusable code?

**Types**

a type is an easy way to refer to the different properties and functions that a value has.

a value is anything we can assign to a variable

“Red” - what is inside this box? it is a string, it is a value that has all the properties + methods that we assume a string has

charAt(), concat(), includes()

```jsx
interface Todo {
    id: number,
    title: string,
    completed: boolean
}
```

here a new Todo type gets added to the ts sytsem - response.datta is an object that has x property, y property- this is inconvenient- isntead we formed a shortcut- response.data is a Todo

every value in Ts has a type

