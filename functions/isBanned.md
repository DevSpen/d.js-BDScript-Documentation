# $isBanned
Returns if the a user is banned from the provided server.

> 'true' means the user is banned, 'false' means the user isn't banned.

## Usage
```
$isBanned[guildID;userID]
```

### Breakdown
`guildID` - The server to get the data from.

`userID` - The user to check.

## Example
```js
bot.command({
    type: "command",
    name: "banned",
    code: `Is <@$message[1]> banned? $isBanned[$guildID;$message[1]].
    $argsCheck[>1;Please provide a userID!]`
})
```
