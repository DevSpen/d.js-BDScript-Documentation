# $channelExists
Checks whether or not the given channel exists. Returns "true" if it exists, returns "false" if it doesn't.

## Usage
```$channelExists[channelID]```

### Breakdown
`channelID` - The channel which the bot checks.

## Example
```
bot.command({
    type: "command",
    name: "channel-exists",
    code: `Channel Exists? $channelExists[$message]`
})
````
