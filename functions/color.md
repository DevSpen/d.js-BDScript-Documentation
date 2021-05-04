# $color
Set an Embed color.

## Usage
```$color[int|hex]```

### Breakdown
`int|hex` - The `int` or `hex` for the color.

## Example
```
bot.command({
    type: "command",
    name: "check-condition",
    code: `$description[I'm cute.]
    $color[ff57e0]
    `
})
```
