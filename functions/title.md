# $title
Sets a title for the embed.

## Usage
```$title[text;(optional) URL]```

### Breakdown
`text` - The text that appears in the title.

`URL` - The title URL hyperlink. Optional.

## Example
```
bot.command({
 type: "command",
 name: "title",
 code: `$title[Hi! This is an example.]`
})
```
