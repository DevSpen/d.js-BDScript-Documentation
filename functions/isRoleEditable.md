# $isRoleEditable
Returns if a role is editable by the bot.
> 'true' means the bot can edit the role, 'false' means it can't.

## Usage
```
$isRoleEditable[guildID;roleID]
```

### Breakdown
`guildID` - The server that the role belongs to.

`roleID` - The role to check.

## Example
```js
bot.command({
    type: "command",
    name: "role-editable",
    code: `$description[Is <@&$findRole[$message]> Editable? $isRoleEditable[$guildID;$findRole[$message]]]`
})
```
