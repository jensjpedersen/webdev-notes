

# Styled Components
* Can use nesting
* Can pass props 


## Install
```bash
npm install --save styled-components
```


## Import
```javascript
import styled from "styled-components";
```


## Props

```javascript


const StyledDiv = styled.div`
  background-color: red;
  color: ${props => props.color};
  padding: 16px;
  
  p {
    font-size: 24px;
  }
`;
```

