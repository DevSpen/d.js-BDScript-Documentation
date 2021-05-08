# $editMessage
Edits the bot's message that has already been sent.

## Usage
```$editMessage[channel ID;message ID;new message;returnMessageID (yes/no) (optional)]```

### Breakdown

`channel ID` - The channel where the message was sent.

`message ID` - The message to edit.

`new message` - The new content of the message.

`returnMessageID` - Whether to return the edited message ID. Default is `no`

## Example
```
bot.command({
    type: "command",
    name: "edit",
    code: `$editMessage[$channelID;123456789101112;Hello]`
})
```
