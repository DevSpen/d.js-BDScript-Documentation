# $channelType
Gets the type of the channel.

## Usage
```$channelType[channelID]```

### Breakdown
`channelID` - The channel which the bot checks.

## Example
```
bot.command({
    type: "command",
    name: "channel-type",
    code: `This channel is $channelTopic[839024362673668117].`
})
````
