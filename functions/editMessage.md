# $editMessage
Edits the bot's message.

## Usage
```$editMessage[channel ID;message ID;new message;returnMessageID (yes/no) (optional)]```


### Breakdown

`channel ID` - The channel where the message was sent.

`message ID` - The message to edit.

`new message` - The new content to edit for this message.

`returnMessageID` - Whether to return the edited message ID. Default is `no`


## Example
```
bot.command({
    type: "command",
    name: "hi",
    code: `
    $channelSendMessage[$channelID;Hi;yes] //'123456789101112' will be the message ID.
    `
})
```

To edit the message,
```
bot.command({
    type: "command",
    name: "edit",
    code: `
    $editMessage[$channelID;123456789101112;Hello]
    `
})
```
