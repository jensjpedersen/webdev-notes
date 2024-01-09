
# UseEffect
* hook used to perform side effects
* uesEffect always runs on the first render



**Parameters**
* callback function: what useEffect will do
* dependency array: what useEffect will listen to: 
  * no dependency array: useEffect will run on every render
  * empty dependency array: useEffect will only run on the first render
  * specific states: useEffect will run when the specific states change


# Side effects
Data fetching, setting up a subscription, and manually changing the DOM in
React components are all examples of side effects. 

Two common types of side effects in React: 
* those that don’t require cleanup 
* those that do.

## Cleanup

# Parameters
## Callback


## Dependency array

### Empty dependency array
* Dependency array: if empty, useEffect will only run on the first render



### Listening to specific states
#### Example
* useEffect listens to changes in `count` state

```javascript

    const [count, setCount] = useState(0); 

    useEffect(() => {
        // Whenever count changes, log count to console. 
        console.log("the count is: ", count);
    }, [count])
    return (
        <>
            <button onClick={() => setCount(count + 1)} >incremnt</button>
            <button onClick={() => setCount(count - 1)} >decrement</button>

            <h3> count: {count}</h3>

        </>
    )
```

