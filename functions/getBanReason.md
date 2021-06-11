# $getBanReason
Gets the reason why a user was banned.


## Usage
```
$getBanReason[guildID;userID]
```

### Breakdown
`guildID` - The server to get the data from.

`userID` - The user to return the data for.


## Example
```js
bot.command({
    type: "command", 
    name: "ban-reason", 
    code: `$onlyIf[$message[1]!=;Please provided a user ID!]
    Reason For <@$message[1]>'s Ban: $getBanReason[$guildID;$message[1]]`
})
```
