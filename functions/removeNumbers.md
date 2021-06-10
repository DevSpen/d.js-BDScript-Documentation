# $removeNumbers
Removes all numbers from the provided text.

## Usage
```
$removeNumbers[text]
```

### Breakdown
`text` - The text to remove numbers from.

## Example
```js
bot.command({
    type: "command", 
    name: "example", 
    code: `$removeNumbers[Hey everyone! 123]`
    // Returns 'Hey everyone!'.
})
```
