# $serverMaximumMembers
This function returns the limit of members a server has. Will return `100000`, unless the server has above 100,000 members.

## Usage
```
$serverMaximumMembers[(optional) guildID]
```

### Breakdown
`guildID` - The server to get the data from. If this field is not inputted, the current server is used.


## Example
```js
bot.command({
    type: "command",
    name: "max-members",
    code: `This server's max member count is: $serverMaximumMembers`
})
```
