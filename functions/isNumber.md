# $isNumber
Returns whether or not the provided 'text' is a number.

## Usage
```
$isNumber[text]
```

### Breakdown
`text` - The text to check.

## Example
```js
bot.command({
    type: "command",
    name: "favorite-number",
    code: `$onlyIf[$isNumber[$noMentionMessage]==true;Only numbers are allowed!]
    <@$authorID>'s favorite number is $noMentionMessage`
})
```
