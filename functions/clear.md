# $clear
Clear an amount of messages in a channel.

## Usage
```$clear[channelID;how many;userID (optional);showTotal (yes/no) (optional)]```

### Breakdown
`channelID` - The ID for this channel.

`how many` - The amount of messages to delete.

`userID` - The ID of the user to delete messages.

`showTotal` - Returns the amount of messages that were actually deleted. Default is `no`.

## Example
```
bot.command({
    type: "command",
    name: "check-condition",
    code: `$clear[$channelID;$message].
    `
})
```
