# $deleteChannelOverwrite
Deletes a channel overwrite.

## Usage
```
$deleteChannelOverwrite[channelID;roleID/userID;reason]
```

### Breakdown
`channelID` - The channel to delete the overwrites for.

`roleID/userID` - The user or role ID to remove the overwrites from.

`reason` - The audit log reason to removing the overwrites. Can be left empty.

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `$deleteChannelOverwrite[$channelID;837400780436275252;Just for fun!]`
})
```
