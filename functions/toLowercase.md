# $toLowercase
Converts text to all lowercase.

## Usage
```
$toLowercase[text]
```

### Breakdown
`text` - The text to convert.

## Example
```js
bot.command({
    type: "command",
    name: "lowercase",
    code: `$toLowercase[$noMentionMessage]`
})
```
