# $serverDescription
Returns the description of the server, if any.

## Usage
```
$serverDescription[(optional) guildID]
```

### Breakdown
`guildID` - The server to get the description from. Uses the current server, if none is provided.

## Example
```js
bot.command({
    type: "command",
    name: "description",
    code: `Server Description: $serverDescription`
})
```
