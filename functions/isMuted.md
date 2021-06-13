# $isMuted
Returns whether or not a user is muted. Applies to both self and server mutes.
> 'true' means the user is muted, 'false' means the user isn't.

### Usage
```
$isMuted[guildID;userID]
```
> You can also use just `$isMuted` without any fields, to return data from the author in the current server.

### Breakdown
`guildID` - The server to get the data from.

`userID` - The user to get the data for.

## Example
```js
bot.command({
    type: "command",
    name: "muted",
    code: `Is <@$mentioned[1;yes]> muted?: $isMuted[$guildID;$mentioned[1;yes]]`
})
```
