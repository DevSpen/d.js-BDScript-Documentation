# $isChannelEditable
Returns whether or not the channel is editable by the bot.
> 'true' means the channel is editable be the bot, 'false' means it isn't.

## Usage
```
$isChannelEditable[(optional) channelID]
```

### Breakdown
`channelID` - The channel to check. Uses the current channel, if none is provided.

## Example
```js
bot.command({
    type: "command",
    name: "editable",
    code: `Is This Channel Editable By Me? $isChannelEditable`
})
```
