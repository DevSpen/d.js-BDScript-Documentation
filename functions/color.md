# $color
Sets the embed's border color.

## Usage
```$color[int of hex]```

### Breakdown
`int or hex` - The `int` or `hex` for the color.

## Example
```
bot.command({
    type: "command",
    name: "color-example",
    code: `$description[I'm cute.]
    $color[ff57e0]`
})
```
[Info Msg] Find color hexes [here](https://htmlcolorcodes.com)!
