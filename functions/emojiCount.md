# $emojiCount
Returns the emoji count from the given server.

## Usage
```$emojiCount[guild ID;type (all/animated/normal)]```

### Breakdown
`guild ID` - The server that the bot returns the emoji count for. Use `$guildID` for the current server.

`type` - Emoji type to count. Type can be `all`, `animated`, or `normal`.

## Example
```
bot.command({
    type: "command",
    name: "emoji-count",
    code: `$emojiCount[$guildID;all] Emojis`
})
```
