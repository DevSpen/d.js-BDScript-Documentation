# $getChannelSlowmode
Gets the slowmode of a channel in seconds.

## Usage
```
$getChannelSlowmode[(optional) channelID]
```

### Breakdown
`channelID` - The channel to return the slowmode for. If no channelID is provided, the bot uses the channel which the command was executed in.

## Example
```
bot.command({
    type: "command",
    name: "check-slowmode",
    code: `The slowmode for this channel is $getChannelSlowmode!`
})
```
