# $getServerVar
Returns a server variable value.

## Usage
```
$getServerVar[variableName;(optional) guildID]
```

### Breakdown
`variableName` - The name of the variable to get.

`guildID` - The server to get the value for. If no guildID is inputted, then the current server is used.

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `There have been $getServerVar[Messages] messages sent in this server.`
})
```
