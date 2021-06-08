# $firstChannelMessageID
Returns the first message ID that was sent in a channel.

## Usage
```
$firstChannelMessageID[channelID (optional)]
```

### Breakdown
`channelID` - The channel to get the first message for.

## Example
```js
bot.command({
    type: "command", 
    name: "example", 
    code: `First message ID of this channel: $firstChannelMessageID`
})
```
