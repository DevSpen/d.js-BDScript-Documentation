# $giveRoles
Give multiple roles to a user.

## Usage
```
$giveRoles[guildID;userID;reason;roleIDs]
```

### Breakdown
`guildID` - The server to give the roles in.

`userID` - The user to give the roles to.

`reason` - The audit-log reason for giving the roles.

`roleIDs` - The roles to give the user. Separate IDs using `;`.

## Example
```js
bot.command({
    type: "joinCommand",
    channel: "39459438494840494",
    code: `<@$authorID> just joined the server!
    $giveRoles[$guildID;$authorID;Gave them the member and announcement ping roles.;2304993284934893;38483274837483473]`
})
```
