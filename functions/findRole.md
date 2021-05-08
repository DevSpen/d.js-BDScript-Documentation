# $findRole
Finds a given role name, ID or mention in a server.

## Usage
```$findChannel[guild ID;role]```

### Breakdown
`guild ID` - The server to find the role in. Use `$guildID` for the current server.

`role` - The role name, ID or mention to find.

## Example
```
bot.command({
    type: "command",
    name: "find-role",
    code: `$findRole[$guildID;$message]`
})
```
