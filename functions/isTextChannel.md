# $isTextChannel
Returns whether or not a channel is a text channel.

## Usage
```
$isTextChannel[channelID]
```

### Breakdown
`channelID` - The channel that the bot checks.

## Example
```js
bot.command({
    type: "command",
    name: "is-text",
    code: `<#$mentionedChannels[1;yes]> Is Text Channel? $isTextChannel[$mentionedChannels[1;yes]]`
})
```
