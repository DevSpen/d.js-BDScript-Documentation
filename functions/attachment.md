# $attachment
Adds an attachment to the bot's message.

## Usage
```$attachment[url;(optional) file name]```

### Breakdown
`url` - The URL that the bot makes the attachment from.

`file name` - Sets the name of the attachment. Optional.

## Example
```
bot.command({
    type: "command",
    name: "cat",
    code: `$attachment[https://cataas.com/cat;cute cat]`
})
```
