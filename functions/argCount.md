# $argCount
Returns the number of arguments (words) in the provided 'text'.

## Usage
```
$argCount[text]
```

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `$argCount[Hello! How are you?]
    // Would return '4'
})
```
