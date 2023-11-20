


# Form tag
The `<form>`  element is a container for different types of input elements,
such as: text fields, checkboxes, radio buttons, submit buttons, etc.


## Attributes
`<form action="#" method="post" id="email-collector">` 

* action - The action attribute defines the action to be performed when the form is submitted.
* method - The method attribute specifies the HTTP method (GET or POST) to be used when submitting the form data.
  [HTML Form Attributes](https://www.w3schools.com/html/html_forms_attributes.asp)

# Fieldset tag
* The `<fieldset>` tag is used to group related elements in a form.
* The `<legend>` tag is used to define a caption for the `<fieldset>`  element.

--------------------------------------------------

# Input elements
* **text** is the default value if the type attribute is not specified


## Input types
**types**
* `<input type="reset">`  - Displays a reset button (for resetting the form)
* `<input type="date" name="date">` - Displays a date input field
* `<input type="color">` - Displays a color input field
* `<input type="file" name="file" id="file">` - Displays a file-select field and a "Browse" button (for uploading a file)
* `<input type="password" name="password" id="password">` - Displays a password field
* `<input type="search" name="search" id="search">` - Displays a search field (for searching for text)


The different input types are as follows:
* button 
* checkbox 
* color 
* date 
* datetime-local 
* email 
* file 
* hidden 
* image 
* month 
* number 
* password 
* radio 
* range 
* reset 
* search 
* submit 
* tel 
* text **(default value)**
* time 
* url 
* week 

### Search
```html
<form action="/action_page.php">
  <label for="gsearch">Search Google:</label>
  <input type="search" id="gsearch" name="gsearch">
  <input type="submit">
</form>
```

**Note:** Remember to set a name for the search field, otherwise nothing will be
submitted. The most common name for search inputs is q.

### Submit
* examples on submit buttons: 
```html
<button class="btn main-btn" type="submit">Submit form</button>
```

```html
<input type="submit" value="Submit form">
```

Button provides more flexibility than input type="submit" because it can be
easily styled and can contain images, icons, and even other HTML elements.



## Input attributes
* **required** - Specifies that an input field must be filled out before submitting the form
* **placeholder** - Specifies a short hint that describes the expected value of an input field 
                Usful for describing what the user should enter in the input field
* name - XXX: Specifies the name of an input element. The name attribute is used to
  reference elements in a JavaScript, or to reference form data after a form is
  submitted.
* minlenght - Specifies the minimum number of characters required in an `<input>`  element
* **pattern** - Specifies a regular expression that an `<input>`  element's value is checked against
  phone number: `<input type="tel" pattern="[0-9]{8}">` 

## Input list attribute - pre-defined options
datalist - The `<datalist>` tag specifies a list of pre-defined options for an `<input>` element.

syntax: `<input list="datalist_id">` 

works with the following input types: text, search, url, tel, email, and password. 

```html
<input list="browsers">
<datalist id="browsers">
    <option value="Internet Explorer">
    <option value="Firefox">
    <option value="Google Chrome">
    <option value="Opera">
    <option value="Safari">
</datalist>
```
            
--------------------------------------------------

# Label tag
* Label tag is used to describe the input field
* **for** attribute is used to connect the label to the input field (id of the input field)
  for=id -> id of the input field
```html
<label for="id-radio">Radio button</label>
<input type="radio" id="id-radio">
```

Clicking on the **label** will select the radio button.


* The <label> element helps improve the accessibility and user experience. 



