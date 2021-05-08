# $endsWith
Checks whether a string ends with the given text.

## Usage
```$endsWith[string;text]```

### Breakdown
`string` - The message to check.

`text` - The text to check if the `string` ends with it.


## Example
```
bot.command({
    type: "command",
    name: "endsWith",
    code: `$endsWith[D.js-BDscript is awesome;awesome]`
})
```
