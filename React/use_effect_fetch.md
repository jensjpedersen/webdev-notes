
# Trix - Key takeaways
* check if data is fetched before creating component
```javascript
{data ? <p>{data}</p> : <p>Loading...</p>}
```
or
```javascript
{data && <p>{data}</p>}
```

* run only on mount - with [] as second argument


# Why use useEffect for data fetching?
* XXX: Why not just use a function?


**Resons:**
## Only run on mount
* with [] as second argument, it will only run when the component **mounts**
Don't run on every render

## Listen to state changes
* fetch data when a state changes, and re-render the component. 

## Cleanup
* possible to add a cleanup function

# Data fetching

## Simple example
* [] argument - only run on mount
* 
```javascript
useEffect(() => {
  async function fetchData() {
    // Fetch data from API
    const response = await fetch('https://api.example.com/data');
    const data = await response.json();
    
    // Update state with fetched data
    setData(data);
  }

  fetchData();
}, []);
```


## Explanatory example
```javascript
import React, { useState, useEffect } from 'react';

function MyComponent() {
  const [data, setData] = useState(null);

  useEffect(() => {
    const fetchData = async () => {
      try {
        // Perform data fetching here
        const response = await fetch('https://api.example.com/data');
        const result = await response.json();
        setData(result);
      } catch (error) {
        console.error('Error fetching data:', error);
      }
    };

    fetchData(); // Call the fetchData function

    // Cleanup function (optional)
    return () => {
      // Cleanup logic (if needed)
    };
  }, []); // Empty dependency array means it runs once on mount

  return (
    <div>
      {/* Render your component using the fetched data */}
      {data ? <p>{data}</p> : <p>Loading...</p>}
    </div>
  );
}

export default MyComponent;
```

