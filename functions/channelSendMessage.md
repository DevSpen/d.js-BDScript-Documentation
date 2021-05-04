# $channelSendMessage
Sends a message to a specific channel.

## Usage
```$channelSendMessage[channelID;message;return messageID (yes/no) (optional)]```

### Breakdown
`channelID` - The channel to send the message too.

`message` - The message that sends.

Optional field: Returns the message ID if set to `yes`.

## Examples
```
bot.command({
    type: "command",
    name: "send-message",
    code: `$channelSendMessage[837405770051223562;Hi!]`
})
```
