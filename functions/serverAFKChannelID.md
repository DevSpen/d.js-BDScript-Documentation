# $serverAFKChannelID
Returns a server’s AFK voice channel ID.

![image](https://user-images.githubusercontent.com/69215413/121972109-4d1cbb00-cd48-11eb-81c2-e64cfc16b9d0.png)

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
