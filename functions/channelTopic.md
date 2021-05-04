# $channelTopic
Returns the channel Topic.

## Usage
```$channelTopic[channelID (optional)]```

### Breakdown
`channelID` - The channel which the bot return's the channel topic for. If this field is left empty, it returns the channel topic of the current channel.

## Example
```
bot.command({
    type: "command",
    name: "channel-topic",
    code: `The topic in this channel is: $channelTopic`
})
````
