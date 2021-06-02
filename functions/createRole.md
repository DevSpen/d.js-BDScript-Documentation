# $createRole
Creates a role.

## Usage
```
$createRole[guildID;reason;name;color;hoisted;mentionable;position;returnRoleID;permissions]
```

### Breakdown
`guildID` - The server to create the role in. Use `$guildID` for the current server.

`reason` - The audit log reason for creating the role. Can be left empty.

`name` - The name of the new role.

`color` - The color of the new role. Optional.

`hoisted` - Whether the role is hoisted or not. 'yes' means the role is displayed separately, 'no' means it isn't. Optional.

`mentionable` - Whether the role will be mentionable by everyone or not. 'yes' means the role will be mentionable to everyone, 'no' means it won't. Optional.

`position` - The position of the role (1 being the top, descending). Optional.

`returnRoleID` - Whether to return the role ID upon successful creation or not. 'yes' means the role ID is returned, 'no' means it isn't. Optional.

`permissions` - The [permissions](https://djsbdscript.gitbook.io/docs/permissions) to grant the role. Separate permissions using `;`. By default all permissions are disabled. Optional.

## Example
```js
bot.command({
    type: "command",
    name: "create-cool",
    code: `$createRole[$guildID;A new cool role!;Cool People;#0000FF]`
})
```
