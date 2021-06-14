# $serverAFKTimeout
Returns a server’s AFK timeout in seconds.

![image](https://user-images.githubusercontent.com/69215413/121972109-4d1cbb00-cd48-11eb-81c2-e64cfc16b9d0.png)

## Usage
```
$serverAFKTimeout[(optional) guildID]
```

### Breakdown
`guildID` - The server to return the data for. Returns the current server's AFK timeout, if no guildID is provided.

## Possible Responses
- `60` - 1 minute
- `300` - 5 minutes
- `900` - 15 minutes
- `1800` - 30 minutes
- `3600` - 1 hour

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `Server AFK Timeout: $serverAFKTimeout`
})
```
