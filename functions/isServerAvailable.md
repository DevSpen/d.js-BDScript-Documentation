# $isServerAvailable
Whether the server is available to access. If it is not available, it indicates a server outage.

## Usage
```
$isServerAvailable[guildID]
```

### Breakdown
`guildID` - The server to check.

## Example
```js
bot.command({
    type: "command",
    name: "check-server",
    code: `$onlyIf[$argCount[$noMentionMessage]>=1;Please provide a serverID!]
    Is $noMentionMessage available?: $isServerAvailable[$noMentionMessage]`
})
```
