# $serverFeatures
Returns the server's features.

## Usage
```
$serverFeatures[(optional) guildID;(optional) separator]
```

### Breakdown
`guildID` - The server to get the features from. Uses the current server, if none is provided.

`separator` - The separator between features. Default is a comma (`, `).

## Example
```js
bot.command({
    type: "command",
    name: "features",
    code: `Features: $serverFeatures`
})
```
