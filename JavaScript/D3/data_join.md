
# Creating a datajoin
```javascript

const svg = d3
      .select('body')
      .append('svg')
      
const arr = [1, 2, 3, 4, 5]

const circles = svg
      .selectAll('circle')
      .data(arr)
```

* We have created a datajoin with the array of numbers:
    * And have the available methods: 
        * .enter()
        * .update()
        * .exit()
        * .merge()




## Enter selection 
* Only triggered when ther is no existing DOM element to bind to the data
* Tiggered on init


XXX: do not append before datajoin - will create a new selection. 
```javascript
svg.append("g")
    .selectAll("circle")
    .data(data)
    .enter()
```



## Update selection
* Triggered when there is an existing DOM element to bind to the data

## Merge selection
* combines the enter and update selections
* **New:** can use `.join()` to create a datajoin and merge selection in one go

# Creating animation 
* When creating elements - eneter selection is triggered
* When updating elements - update selection is triggered

Produces duplicated logic




## Example animation: Enter + Update selection 

```javascript
    let circles = svg.selectAll("circle").data(data); 

    // Enter selection - on init:  
    // * here we create the elements
    // * And set initial frame
    // * only triggered on first datajoin selection 
    circles
        .enter()
        .append("circle")
        .attr("cx", d => d.x  )
        .attr("cy", d => d.y + t*10  )
        .attr("r", 5)
        .style("fill", "#69b3a2")
        
        // Duplicate for enter and update selection
        .attr("cx", d => d.x  )
        .attr("cy", d => d.y * Math.sin(t/20)  )


    // Calls update selection
    // * Previous attributes is set
    circles
        .attr("cx", d => d.x  )
        .attr("cy", d => d.y * Math.sin(t/20)  )
```


XXX: To prevent duplicated logic - we can use the merge selection 
## Example - Merge selection 

Merge: 
```javascript
circles.merge(circlesEnter)
```

**On init - enter selection is triggered (`circlesEnter`), on update - update selection (`circles`) is triggered.**

Merge selection effectively combines the enter and update selection
* update selection - `const circles = svg.selectAll("circle").data(data); // Update selection ` 
* enter selection - `const circlesEnter = circles.enter() // Enter selection` 


```javascript

const circles = svg.selectAll("circle").data(data); // Update selection 
const circlesEnter = circles.enter() // Enter selection
    .append("circle")
    .attr("r", 5)
    .style("fill", "#69b3a2")

// Merge selection
// * Use to prevent duplicate code
// * Merge selection is used for both Enter and  Update selection
circles.merge(circlesEnter)
   .attr("cx", d => d.x  )
   .attr("cy", d => d.y * Math.sin(t/20))
```

## Exampel - New join() method
**Join method = Merge - Enter and Update slection**
* Same as merge selection - but in one go

* Have removed `append("circle")` 
* Use `.join("circle")` instead 
```javascript

let circles = svg.selectAll("circle").data(data); 

circles
    .join("circle")
    .attr("r", 5)
    .style("fill", "#69b3a2")
    .attr("cx", d => d.x  )
    .attr("cy", d => d.y * Math.sin(t/20))

```


