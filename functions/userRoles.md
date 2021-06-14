# $userRoles
Gets a user's roles.

## Usage
```
$userRoles[guildID;userID;option;(optional) separator;(optional) sort (yes/no)]
```

### Breakdown
`guildID` - The server to get the data from.

`userID` - The user to get the roles for.

`option` - What role-data piece to return. Default is `name`. [(see all role properties)](https://djs-bdscript.gitbook.io/docs/properties/role-properties)

`separator` - The separator between each role-data piece, default is `, `.

`sort` - Whether or not to sort the roles by position, default is `no`.

## Example
```js
bot.command({
    type: "command",
    name: "roles",
    code: `$userTag[$mentioned[1;yes]]'s Roles: $userRoles[$guildID;$mentioned[1;yes]]`
})
```
