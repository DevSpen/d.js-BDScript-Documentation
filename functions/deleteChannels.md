# $deleteChannels
Deletes channel(s) from a server.

## Usage
```$deleteChannels[guildID;channelIDs]```

### Breakdown
`guildID` - The server to delete the channels in. Use `$guildID` for current server.

`channelIDs` - The channel's ID(s) to delete, separated by `;`.

## Example
```
bot.command({
    type: "command",
    name: "delete-channel",
    code: `$deleteChannels[$guildID;$mentionedChannels[1;yes]]
    Channel was deleted!`
})
```
