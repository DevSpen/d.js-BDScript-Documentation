# $serverBoostLevel
Returns what Nitro Boost level a server is at.

> 2 Boosts = Level #1
>
> 15 Boosts = Level #2
>
> 30 Boosts = Level #3
>
> The bot returns: `0` (no-boosts), `1`, `2`, or `3`.

## Usage
```
$serverBoostLevel[(optional) guildID]
```

### Breakdown
`guildID` - The server to return the boost level for.

## Example
```js
bot.command({
    type: "command", 
    name: "boost-level", 
    code: `Our current boost level is $serverBoostLevel!`
})
```
