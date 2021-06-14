# $serverMembers
Returns the members of a server.

[WarningMsg] This function may be unstable depending on how large the server is.

## Usage
```
$serverMembers[guildID;option;(optional) separator;(optional) includeBots (yes/no)]
```

### Breakdown
`guildID` - The server to get the members from.

`option` - What to data to return for the users. (e.g `mention`, `name`, `id`)

`separator` - What to separate the users with. Default is a comma (`, `).

`includeBots` - Whether to include bots or not. Default is `yes`.

## Example
```js
bot.command({
    type: "command",
    name: "member-ids",
    code: `Members: $serverMembers[$guildID;id]`
})
```


