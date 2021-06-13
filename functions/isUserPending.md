# $isUserPending
Whether or not a user has yet to pass the server's [membership screening](https://support.discord.com/hc/en-us/articles/1500000466882-Rules-Screening-FAQ).
> 'true' means the user is pending, 'false' mean the user isn't pending.

## Usage
```
$isUserPending[guildID;userID]
```

### Breakdown
`guildID` - The server to get the data from.

`userID` - The user to get the data from.

## Example
```js
  bot.command({
    type: "command", 
    name: "pending", 
    code: `Is <@$message[1]> pending? $isUserPending[$guildID;$message[1]]
    $onlyIf[$argCount[$message]>=1;Please provide a userID!]`
})
```
