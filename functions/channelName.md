# $channelName
Gets the Name of the Given Channel ID.


## Usage
`$channelName[channelID]`


### Breakdown
`channelID` - The ID of the Channel that you want to retrieve the Name.


## Example
```bot.command({
 type: "command",
 name: "channel-name",
 code: `The Channel Name of $message: $channelName[$message]`
 })````
