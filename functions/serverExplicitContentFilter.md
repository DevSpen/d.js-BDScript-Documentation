# $serverExplicitContentFilter
The explicit content filter level of the server. [(see explicit content filter levels)](https://djs-bdscript.gitbook.io/docs/properties/explicit-content-filter-levels)

## Usage
```
$serverExplicitContentFilter[(optional) guildID]
```

### Breakdown
`guildID` - The server to return the data for. Uses the current server, if none is provided.

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `Server Explicit Content Filter: $serverExplicitContentFilter`
})
```
