
# Animation
An animation lets an element gradually change from one style to another.


* Create animation with - `animation` property with 8 sub-properties 

## Animation properties

Can specify in one line:  
```
animation: name duration timing-function delay iteration-count direction fill-mode play-state;
```

or multiple lines 

* animation-name - Name of the animation. Targeted by `@keyframes` rule. 
* animation-duration 
* animation-timing-function 
    * ease - Specifies an animation with a slow start, then fast, then end slowly (this is default)
    * linear - Specifies an animation with the same speed from start to end
    * ease-in - Specifies an animation with a slow start
    * ease-out - Specifies an animation with a slow end
    * ease-in-out - Specifies an animation with a slow start and end
    * cubic-bezier(n,n,n,n) - Lets you define your own values in a cubic-bezier function
  
* animation-delay: 
    * animation-iteration-count 
    * number	A number that defines how many times an animation should be played. Default value is 1	
    * infinite	Specifies that the animation should be played infinite times (for ever)	
    * initial	Sets this property to its default value. Read about initial	
    * inherit	Inherits this property from its parent element. Read about inherit

* animation-direction: 
    * normal - The animation is played as normal (forwards). This is default
    * reverse - The animation is played in reverse direction (backwards)
    * alternate - The animation is played forwards first, then backwards
    * alternate-reverse - The animation is played backwards first, then forwards
  
* animation-fill-mode: 
    * none - Default value. Animation will not apply any styles to the element before or after it is executing
    * forwards - The element will retain the style values that is set by the last keyframe (depends on animation-direction and animation-iteration-count)
    * backwards - The element will get the style values that is set by the first keyframe (depends on animation-direction), and retain this during the animation-delay period
    * both - The animation will follow the rules for both forwards and backwards, extending the animation properties in both directions
* animation-play-state: 







# Keyframes 

* `from`  is not necessary, because the animation will start from the current style (red).

```css
/* The animation code */
@keyframes example {
  from {background-color: red;}
  to {background-color: yellow;}
}

/* The element to apply the animation to */
div {
  width: 100px;
  height: 100px;
  background-color: red;
  animation-name: example;
  animation-duration: 4s;
}
```

* In this case, `from` is not necessary, because the animation will start from
the current style (red).

**Sorthand**
```css
div {
  animation: example 4s;
}
```


## Change to multiple states during the animation
```css
@keyframes example {
  0%   {background-color:red; left:0px; top:0px;}
  25%  {background-color:yellow; left:200px; top:0px;}
  50%  {background-color:blue; left:200px; top:200px;}
  75%  {background-color:green; left:0px; top:200px;}
  100% {background-color:red; left:0px; top:0px;}
}
```




