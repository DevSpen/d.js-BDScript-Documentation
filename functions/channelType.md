# $channelType
Gets the type of the channel.

## Usage
```$channelType[(optional) channelID]```

### Breakdown
`channelID` - The channel which the bot checks. Uses current channel, if nothing is provided.

### Possible Channel Types
- `dm` - A DM channel
- `text` - A text channel.
- `voice` - A voice channel.
- `category` - A category.
- `news` - A announcement/news channel.
- `store` - A store channel.
- `stage` - A stage channel.
- `unknown` - Other.

## Example
```js
bot.command({
    type: "command",
    name: "channel-type",
    code: `This channel is a $channelType channel.`
})
````
