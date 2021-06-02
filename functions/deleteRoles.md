# $deleteRoles
Deletes role(s) from a server.

## Usage
```
$deleteRoles[guildID;roles]
```

### Breakdown
`guildID` - The ID of the server to delete the role(s) in. Use `$guildID` for the current server.

`roles` - The ID(s) of the role(s) to delete. Separate role IDs using `;`.

## Example
```js
bot.command({
    type: "command",
    name: "delete-role",
    code: `$deleteRoles[$guildID;$findRole[$message]]
    Deleted role "$roleName[$findRole[$message]]"!
    $onlyIf[$hasPerm[$guildID;$authorID;manageroles]==true;You need the manage roles permission to use that!]`
})
```
