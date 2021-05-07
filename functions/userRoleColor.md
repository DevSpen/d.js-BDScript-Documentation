# $userRoleColor
Displays the user's highest role color.

## Usage #1
`$userRoleColor[guildID;userID]` - Gets a user's highest role with the provided data.

### Breakdown
`guildID` - The guild to get the user's highest role color from.

`userID` - The user to get the highest color from.

## Usage #2
`$userRoleColor` - Returns the author's highest role color from the current server.

## Example
```
bot.command({
    type: "command",
    name: "user-color",
    code: `$username[$mentioned[1;yes]]'s highest role color is: **$userRoleColor[$guildID;$mentioned[1;yes]]**`
})
````
