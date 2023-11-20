
# Nodeman
* Nodeman auto restarts nodejs process when file changed.

install nodeman

`npm install -g nodeman`
## auto add to package.json
```bash
npm i -install-save-dev nodeman
```
Then add 
`"devStart": "nodemon server.js"` 
to script section in package.json


## Usage
`nodeman server.js`
