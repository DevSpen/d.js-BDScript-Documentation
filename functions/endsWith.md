# $endsWith
Checks whether a string ends with a given text.

## Usage
```$endsWith[message;text]```

### Breakdown

`message` - The message to check.

`text` - The text to check if the `message` ends with text.


## Example
```
bot.command({
    type: "command",
    name: "endsWith",
    code: `
    Does 'D.js-BDscript is awesome' ends with 'awesome'? 
    $endsWith[D.js-BDscript is awesome;awesome] //Returns 'true'.
    `
})
```
