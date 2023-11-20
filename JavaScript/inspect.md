
# Firefox debug


# Node debug
* Debugging server-side JavaScript with Node.js and Chrome DevTools

## Lucnh node with inspect flag
```javascript
NODE_INSPECT_RESUME_ON_START=1 nodemon inspect script.js
```

## Open chrome devtools

* Open chrome dev tools
1. 
chrome://inspect/
or 
about:inspect

2. click "Open dedicated DevTools for Node"

## Disable autofocus sources panel
* In the Chrome DevTools Settings under Preferences -> Sources, there is an option "Focus Sources panel when triggering a breakpoint". Disabling this option seems to fix the issue.

## Disable autfocus chrome
* chrome://flags/#enable-devtools-experiments


## Run node with debug flag

