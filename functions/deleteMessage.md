# $deleteMessage
Deletes the message provided.

## Usage
```$deleteMessage[ChannelID;MessageID]```

### Breakdown
`ChannelID` - ID of the channel where the target message is located.

`MessageID` - ID of the target message.

## Example
```
bot.command({
   type: "command"
   name: "test"
   code: `$deleteMessage[837400203878596651;839088754441453578]
           Deleted the message!`
})
```
[Tip Msg] You can use multiple `$deleteMessage` in one command.
