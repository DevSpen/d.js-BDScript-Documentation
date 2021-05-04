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
    code: `This channel is a $channelType[839024362673668117] channel.`
})
````
