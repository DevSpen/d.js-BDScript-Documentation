# $findServerChannel
Finds a channels in a given server using name, ID or mention.

## Usage
```$findServerChannel[guild ID;channel;returnChannelID (optional)]```

### Breakdown
`guild ID` - The server to find the channel in.

`channel` - The channel `name`, `ID` or `mention` to find.

`returnChannelID` - Whether to return the current channel ID if there is no channel found.

## Example
```
bot.command({
    type: "command",
    name: "find-channelin",
    code: `$findServerChannel[$message[1];$message[2]]`
})
```
[Info Msg] The bot must inside the given server to find the channel.
