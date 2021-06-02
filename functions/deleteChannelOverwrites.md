# $deleteChannelOverwrites
Deletes all overwrites for the provided channel.

## Usage
```
$deleteChannelOverwrites[channelID;reason]
```

### Breakdown
`channelID` - The channel to remove the overwrites for.

`reason` - The audit log reason to removing the overwrites. Can be left empty.

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `$deleteChannelOverwrites[$channelID;Just for fun!]`
})
```
