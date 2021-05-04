# $channelTopic
Returns the channel Topic.

## Usage
```$channelTopic[channelID (optional)]```

### Breakdown
`channelID` - The channel which the bot checks.

## Example
```
bot.command({
    type: "command",
    name: "channel-topic",
    code: `The topic in this channel is: $channelTopic`
})
````
