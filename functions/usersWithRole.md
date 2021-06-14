# $usersWithRole
Returns a list of users with the provided role.

## Usage
```
$usersWithRole[guildID;roleID;(optional) option;(optional) separator]
```

### Breakdown
`guildID` - The server to get the role from.

`roleID` - The role to get the users from.

`option` - The data to return about the users. Default is `username`. Valid options: `username`, `mention`, `id`, `discriminator`, `count`, etc.

`separator` - The separator between each user-data piece, default is `, `.

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `$usersWithRole[$guildID;837619299383771167;id]`
})
```

