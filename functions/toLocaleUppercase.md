# $toLocaleUppercase
Turns first letter of the provided words uppercase.

## Usage
```$toLocaleUppercase[text]```

### Breakdown
`text` - The text to convert.

## Example
```
bot.command({
 type: "command",
 name: "locale-uppercase",
 code: `$toLocaleUppercase[$message]`
})
```
