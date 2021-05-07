# $emojiCount
Returns the emoji count from the given server.

## Usage
```$emojiCount[guild ID;type (all/animated/normal)]```


### Breakdown

`guild ID` - The server ID to count the emojis.

`type` - Emoji type to count. Type can be `all`, `animated`, `normal`.


## Example
```
bot.command({
    type: "command",
    name: "emojis-count",
    code: `
    $emojiCount[$guildID;all] //Returns the emoji count from the current server.
    `
})
```
