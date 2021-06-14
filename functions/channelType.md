# $channelType
Gets the type of the channel.

### What are the channel types?
[PageURL:Channel Types]()

## Usage
```$channelType[(optional) channelID]```

### Breakdown
`channelID` - The channel which the bot checks. Uses current channel, if nothing is provided.

## Example
```js
bot.command({
    type: "command",
    name: "channel-type",
    code: `This channel is a $channelType channel.`
})
````
