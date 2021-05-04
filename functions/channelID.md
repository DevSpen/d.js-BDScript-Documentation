# $channelID
This Function will return the ID of the given Channel Name.


## Usage
`$channelID[channelName]`

### Breakdown
`channelName` - The name of the Channel for which you want to retrieve the ID.

## Example
```bot.command({
 type: "command",
 name: "channel-id",
 code: `Channel ID of $message: $channelID[$message]`
 })````
