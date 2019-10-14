make a network request to fetch some json and print the result

create new project directory- create package.json - install anxios to make a request - write code

axios used to make a network request

jsonplaceholder.typicode.com /todos

chrome extension to format json

```jsx
mkdir fetchjson
cd fetchjson
npm init -y // genrates the package.json
npm install axios 
```

create new file inside project called index.ts short for typescript

```jsx
import axios from 'axios'

const url = 'https://jsonplaceholder.typicode.com/todos/1'

// receive a promise
axios.get(url).then(response => {
    console.log(response.data);
})
```

need to comile to js first

inside terminal

```jsx
tsc index.ts
```

this compiels the file- in editor new file index.js will appear - this is the compiled version of our code

```jsx
node index.js
```

To combine these commands into one can use ts-node automatically comiples and executes

```jsx
ts-node index.ts
```

**one quick change**

```jsx
import axios from 'axios'

const url = 'https://jsonplaceholder.typicode.com/todos/1'

// receive a promise
axios.get(url).then(response => {
    const {todo} = response.data;
    
    const ID = todo.ID
    const title = todo.Title
    const finished = todo.finished
    
    console.log(`the todo with ID ${ID} has a title of ${Title}`)
    
})
```

try running the file and will get console.log undefined undefined undefined

**catching errors**

we wrote some code but didnt know what we did wrong until we executed the code

would be nice to have a comment in the code like

```jsx
// Response.data has properties of:
// id
// title
// completed
```

in ts form… also including the type of data each proerties contains

```jsx
interface Todo {
    id: number,
    title: string,
    completed: boolean
}
```

interfaces are used to define the structure of an object . we can ignore proeprties in interfaces if we want to

```jsx
import axios from 'axios'

const url = 'https://jsonplaceholder.typicode.com/todos/1'

interface Todo {
    id: number,
    title: string,
    completed: boolean
}

axios.get(url).then(response => {
    const {todo} = response.data as Todo;
    
    const ID = todo.ID
    const title = todo.Title
    const finished = todo.finished
    
    console.log(`the todo with ID ${ID} has a title of ${Title}`)
    
})
```

ts shows us some syntax errors and gives us messages

**catching more errors **

```jsx
logTodo(id, completed, title)

const logTodo = (id, title, completed) => {
    console.log(id, title, completed)
}
```

passed in the arguments in the wrong order

using ts.. using annotators

```jsx
const logTodo = (id: number, title: string, completed: boolean) => {
    console.log(id, title, completed)
}
```



