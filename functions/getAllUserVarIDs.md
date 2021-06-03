# $getAllUserVarIDs
Returns all the provided server's user IDs that have at least one variable value assigned in the database.

## Usage
```
$getAllUserVarIDs[guildID;separator (optional)]
```

### Breakdown
`guildID` - The server to get the IDs from.

`separator` - The separator between each ID.

## Example
```
bot.command({
    type: "command",
    name: "example",
    code: `$getAllUserVarIDs[$guildID]
    $onlyForIDs[$botOwnerID;Only my owner can use that!]`
})
```
