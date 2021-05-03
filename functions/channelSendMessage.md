# $channelSendMessage
Sends a message to a specific channel.

## Usage
```$channelSendMessage[channelID;message]```

### Breakdown
`channelID` - The channel to send the message too.

`message` - The message that sends.

## Examples
```
bot.command({
    type: "command",
    name: "send-message",
    code: `$channelSendMessage[837405770051223562;Hi!]`
})
```
