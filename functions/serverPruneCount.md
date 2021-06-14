# $serverPruneCount
Returns the amount of members that will be kicked after pruning.

## Usage
```
$serverPruneCount[guildID;(optional) days;(optional) roles]
```

### Breakdown
`guildID` - The server to get the prune data from.

`days` - How many days of inactivity a user needs to be included in the count. Default is `7`. (`30` is max, `1` is minimum)

`roles` - The roles to ignore. If the inactive user has one of these roles, they will not be included in the count. Default is none.

## Example
```js
bot.command({
    type: "command",
    name: "test-prune",
    code: `If this server was pruned, $serverPruneCount[$guildID] members would be kicked.`
})
```
