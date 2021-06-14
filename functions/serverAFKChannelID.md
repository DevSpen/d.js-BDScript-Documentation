# $serverAFKChannelID
Returns a server’s AFK voice channel ID.

## Usage
```
$serverAFKChannelID[(optional) guildID]
```

### Breakdown
`guildID` - The server to return the data for. Returns the current server's AFK channelID, if no guildID is provided.

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `Server AFK Channel: <#$serverAFKChannelID>`
})
```
