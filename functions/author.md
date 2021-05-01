# $author
Sets the author text, icon, and/or URL.

## Usage
`$author[text;image url;hover url]`

[Info Msg] All fields in `$author[]` are optional.

### Breakdown
`text` - Sets author text.

`image url` - Sets author icon.

`hover url` - Sets clickable URL. This only works if the text field is inputted.

## Example
```
bot.command({
    type: "command",
    name: "author",
    code: `$author[This is the author text.;https://cataas.com/cat;https://bit.ly/djs-bdscript]`
})
```
