# $isRoleManaged
Returns if a role is managed by a external service (e.g a automatically created integration or server booster role).
> 'true' means the role is managed, 'false' means it isn't.

## Usage
```
$isRoleManaged[guildID;roleID]
```

### Breakdown
`guildID` - The server that the role belongs to.

`roleID` - The role to check.

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `$description[Is <@&$findRole[$message]> Managed? $isRoleManaged[$guildID;$findRole[$message]]]`
})
```
