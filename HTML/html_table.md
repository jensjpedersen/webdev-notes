
# Html table

* table cell / table element `<td></td>`  (table data)
* tr - table row 
* th - table header


# Structure

* <table>



# Tags
* <table>	Defines a table
* <th>	Defines a header cell in a table
* <tr>	Defines a row in a table
* <td>	Defines a cell in a table
* <caption>	Defines a table caption
* <colgroup>	Specifies a group of one or more columns in a table for formatting
* <col>	Specifies column properties for each column within a <colgroup> element
* <thead>	Groups the header content in a table
* <tbody>	Groups the body content in a table
* <tfoot>	Groups the footer content in a table
* 

# td element
 ## Attributes
* colspan - Specifies the number of columns a cell should span
`<th colspan="8"></th>` 



XXX: 
* colspan vs span 


# Colgroup
* Used to style columns in a table
* Colgroup is used to group columns in a table

**Note:** The <colgroup> tag must be a child of a <table> element, after any
<caption> elements and before any <thead>, <tbody>, <tfoot>, and <tr> elements.

Example: 
```css
<table>
  <colgroup>
    <col span="2" style="background-color:red">
    <col style="background-color:yellow">
  </colgroup>
  <tr>
    <th>ISBN</th>
    <th>Title</th>
    <th>Price</th>
  </tr>
  <tr>
    <td>3476896</td>
    <td>My first HTML</td>
    <td>$53</td>
  </tr>
</table>
```

* sets first two columns to red and the third to yellow

## Attributes
* **span**	- Specifies the number of columns a column group should span

