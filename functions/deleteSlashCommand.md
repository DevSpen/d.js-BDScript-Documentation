# $deleteSlashCommand
Deletes a slash command globally or for a server.

## Usage
```
$deleteSlashCommand[global/guildID;name/ID]
```

### Breakdown
`global/guildID` - If `global` is inputted, then the slash command is deleted in all servers. If a `guildID` is provided, then the bot will delete the slash command for that server.

`name/ID` - The name or ID of the slash command, that the bot will delete.

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `$deleteSlashCommand[global;testSlash]
    $onlyForIDs[$botOwnerID;Only my owner can use that!]`
})
```
