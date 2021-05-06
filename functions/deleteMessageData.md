# $deleteMessageData
Deletes all the variable values for given message.

## Usage
```$deleteMessageData[messageID]```

### Breakdown
`messageID` - The message to delete the data from. 

## Example
```
bot.command({
 type: "command",
 name: "deletemsgdata",
 code: `$deleteMessageData[$message]
 Deleted all the data from message: $message!`
 })
 ```
