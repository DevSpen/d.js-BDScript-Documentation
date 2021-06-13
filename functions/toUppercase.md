# $toUppercase
Converts text to all uppercase.

## Usage
```
$toUppercase[text]
```

### Breakdown
`text` - The text to convert.

## Example
```js
bot.command({
    type: "command",
    name: "uppercase",
    code: `$toUppercase[$noMentionMessage]`
})
```
