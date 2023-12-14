

# Input fields - important!!!
* When working with user text, do not use innerHTML. Use textContent in stead. 
* A user can enter html and execute javascript if you use innerHTML.  This is
  called a cross site scripting attack.  Use textContent instead.  It will
  escape the html and javascript.  It will not execute it.
