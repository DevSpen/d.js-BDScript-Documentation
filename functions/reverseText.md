# $reverseText
Reverses the provided text.

## Usage
```
$reverseText[text]
```

### Breakdown
`text` - The text to reverse.

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `$reverse[hello]`
  // Returns 'olleh'
})
```
