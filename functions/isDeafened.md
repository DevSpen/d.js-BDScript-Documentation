# $isDeafened
Returns whether or not a user is deafened. Applies to both self and server deafen.
> 'true' means the user is deafened, 'false' means the user isn't.

### Usage
```
$isServerDeafened[guildID;userID]
```
> You can also use just `$isDeafened` without any fields, to return data from the author in the current server.

## Breakdown
`guildID` - The server to get the data from.

`userID` - The user to get the data for.

## Example
```js
bot.command({
    type: "command",
    name: "respects",
    code: `Is <@$mentioned[1;yes]> deafened?: $isDeafened[$guildID;$mentioned[1;yes]]`
})
```
