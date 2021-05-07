# $takeRoles
Removes role(s) from an user in a certain server.

## Usage
```$takeRoles[guildID;userID;reason;roles]```

### Breakdown
`guildID` - The server where the role(s) will be removed.

`userID` - The user that the role(s) get removed from.

`reason` - The reason why the role(s) are getting removed from the user. (for audit logs)

`roles` - The ID of every role you want to take from the user, separated by `;`.

## Example
```
bot.command({
 type: "command",
 name: "remove-role",
 code: `$takeRoles[$guildID;$findUser[$message[1]];Role removed by $username ($authorID).;$findRole[$message[2]]
 Removed $roleName[$findRole[$message[2]]] from <@$findUser[$message[1]]>.
 $onlyIf[$findRole[$message[2]]!=;Could not find role!]
 $onlyIf[$hasPerm[$guildID;$authorID;manageroles]==true;You need the manage roles permission to use that!]
 $onlyIf[$findUser[$message[1]]!=$authorID;Could not find user!]`
})
```
