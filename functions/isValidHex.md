# $isValidHex
Checks whether or not the provided [color hex](https://htmlcolorcodes.com/color-picker) is valid.
> 'true' means the color hex is valid, 'false' means it isn't.

## Usage
```
$isValidHex[colorHex]
```

### Breakdown
`colorHex` - The color hex to check.

## Example
```js
  bot.command({
    type: "command", 
    name: "check-hex", 
    code: `$onlyIf[$argCount[$noMentionMessage]>=1;Please provide a *color hex*!]
    Is $noMentionMessage a valid hex?: $isValidHex[$noMentionMessage]`
})
```
