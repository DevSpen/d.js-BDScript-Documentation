# $deleteMessage
Deletes the message of provided Message ID

## Usage
```$deleteMessage[ChannelID;MessageID]```

### Breakdown
`ChannelID` - ID of the Channel where the target message is located.

`MessageID` - ID of the target message.

## Example
```
bot.Command({
   type: "command"
   name: "test"
   code: `$deleteMessage[837400203878596651;839088754441453578] //Deletes the message 839088754441453578 from the channel 837400203878596651
           Deleted the message!`
})
```

#### Notices
[Info Msg] You can use multiple `$deleteMessage` in one command.
