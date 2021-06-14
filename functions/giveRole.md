# $giveRole
Gives a role to a user.

## Usage
```
$giveRole[guildID;userID;roleID;reason]
```

### Breakdown
`guildID` - The server to give the role in. Use `$guildID` for the current server.

`userID` - The user to give the role to.

`roleID` - The role to give to the user.

`reason` - The audit-log reason for giving the role.

## Example
```js
bot.command({
    type: "joinCommand",
    channel: "39459438494840494",
    code: `<@$authorID> just joined the server!
    $giveRole[$guildID;$authorID;93478932783473848;Give them the member role.]`
})
```

