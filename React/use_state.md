
# State managment
**Used to update state, render component agian, and update UI**

**It only affects what useState will return starting from the next render.**:
* hence do not call set function in js code. 



## useState() - count example

* setCount - reference to the function that will update the state
* count - the current state value


```javascript
import { useState } from 'react';

function App() {
  // Declare a new state variable, which we'll call "count"
  const [count, setCount] = useState(0);
  
  const increment = () => {
    setCount((count) => count + 1);
  };
  
  return (
    <>
      <button onClick={increment}>increment</button>
    </>
  );
}
```





# useState

useState is a React Hook that lets you add a state variable to your **component**.

```javascript
const [state, setState] = useState(initialState);
```
The convention is to name state variables like [something, setSomething] using array destructuring.


**Parameters**
* initialState: The value you want the state to be initially. It can be a value
  of any type, but there is a special behavior for functions. This argument is
  ignored after the initial render.
    * If you pass a function as initialState, it will be treated as an
      initializer function. It should be pure, should take no arguments, and
      should return a value of any type. React will call your initializer
      function when initializing the component, and store its return value as
      the initial state. See an example below.


**Returns**
useState returns an array with exactly two values:

* The current state. During the first render, it will match the initialState
  you have passed.
* The set function that lets you update the state to a different value and
  trigger a re-render.



**Caveats**
* useState is a Hook, so you can only call it at the top level of your
  component or your own Hooks. You can’t call it inside loops or conditions

## setState function 
**setState function**
* set functions do not have a return value.

```javascript
const [name, setName] = useState('Edward');

function handleClick() {
  setName('Taylor');
  setAge(a => a + 1);
}
```


**Caveats**
* The set function only updates the state variable for the next render. If you
read the state variable after calling the set function, you will still get the
old value that was on the screen before your call.


# Usage
Adding state to a component 
Call useState at the top level of your component to declare one or more state variables.


```javascript

import { useState } from 'react';

function MyComponent() {
  const [age, setAge] = useState(42);
  const [name, setName] = useState('Taylor');
  // ...
```

* The convention is to name state variables like [something, setSomething] using array destructuring.

useState returns an array with exactly two items:

* The current state of this state variable, initially set to the initial state you provided.
* The set function that lets you change it to any other value in response to interaction.

To update what’s on the screen, call the set function with some next state:

```javascript

function handleClick() {
  setName('Robin');
}
```

React will store the next state, render your component again with the new
values, and update the UI.



# Trouble shooting

Suppose the age is 42. This handler calls setAge(age + 1) three times:

```javascript
function handleClick() {
  setAge(age + 1); // setAge(42 + 1)
  setAge(age + 1); // setAge(42 + 1)
  setAge(age + 1); // setAge(42 + 1)
}
```
However, after one click, age will only be 43 rather than 45! This is because
calling the set function does not update the age state variable in the already
running code. So each setAge(age + 1) call becomes setAge(43).

## Solution

To solve this problem, you may pass an updater function to setAge instead of the next state:

```javascript
function handleClick() {
  setAge(a => a + 1); // setAge(42 => 43)
  setAge(a => a + 1); // setAge(43 => 44)
  setAge(a => a + 1); // setAge(44 => 45)
}
```
* check [useState – React](https://react.dev/reference/react/useState) for explanation
