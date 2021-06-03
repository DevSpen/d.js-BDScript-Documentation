# $findNumbers
Returns all numbers found in the provided text.

## Usage
```
$findNumbers[text]
```

### Breakdown
`text` - The text that the numbers are pulled from.

## Example
```js
bot.command({
    type: "command",
    name: "find-numbers",
    code: `$findNumbers[$message]`
    // Example: If the message was 'Hi 123', the bot would return '123'.
})
