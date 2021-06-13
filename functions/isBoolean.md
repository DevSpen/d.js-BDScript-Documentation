# $isBoolean
Checks whether or not provided 'text' is a boolean. 

- Accepted Booleans: `on`, `off`, `true`, `false`, `enable`, `disable`, `yes`, `no`.
- Returns 'true' if the text is a valid boolean, otherwise, 'false' is returned.

## Usage
```
$isBoolean[text]
```

### Breakdown
`text` - The text to check.

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `$onlyIf[$argCount[$noMentionMessage]>=1;Please provide text!]
    Is $noMentionMessage boolean? $isBoolean[$noMentionMessage]`
})
```
