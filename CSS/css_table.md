


# Css styling table 
```css

* {
margin: 0;
padding: 0; 
box-sizing: border-box;
}

%% tagete flere elementer med samme styling

table, th, td {
border: 2px solid white; 

%% Collapse border mellom hver celle sammen
border-collapse: collapse; 

text-align: center; 
}


%% legger til extra styling på table
table {
width: 100%
max-width: 800px;
margin-top: 50px;
margin-inline: auto; 
background-color: grey; 
}


Legger til padding på th

th {
padding: 12px; 

}

td {

padding: 20px; 

}


