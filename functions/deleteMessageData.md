# $deleteMessageData
Deletes all the variable values for given message.


## Usage
`$deleteMessageData[messageID]`


### Breakdown
`messageID` - The message to delete the data from. 


## Example
```bot.command({
 type: "command",
 name: "deletemsgdata",
 code: `$deleteMessageData[7391293339239]
Deleted all the data from message $message!`
 })````
