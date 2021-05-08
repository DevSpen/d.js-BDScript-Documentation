Gets a channel's name.

## Usage
```$channelName or $channelName[channelID]```

### Breakdown
Optional field: `channelID` - The ID for this channel. If no channel is provided, it returns the name of the channel the command was ran in.

## Example
```
bot.command({
    type: "command",
    name: "channel-name",
    code: `You are currently in $channelName! Enjoy.`
})
```

Using channel ID
```
bot.command({
    type: "command",
    name: "channel-name",
    code: `Here's the channel name: $channelName[$mentionedChannels[1;yes]]`
})
```
