# $findChannel
Finds a channel from given channel name, ID, or mention.

## Usage
```$findChannel[channel;returnChannelID (yes/no)]```

### Breakdown
`channel` - The channel name/ID/mention to find.

`returnChannelID` - Whether to return the current channel ID if no channel was found.

## Example
```
bot.command({
    type: "command",
    name: "find-channel",
    code: `$findChannel[$message;yes]`
})
```
