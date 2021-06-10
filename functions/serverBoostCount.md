# $serverBoostCount
Returns how many Nitro Boosts a server has.

## Usage
```
$serverBoostCount[(optional) guildID]
```

### Breakdown
`guildID` - The server to return the boost count for. If nothing is provided, the bot uses the current server.

## Example
```js
bot.command({
    type: "command", 
    name: "boost-count", 
    code: `We currently have $serverBoostCount boosts!`
})
```
