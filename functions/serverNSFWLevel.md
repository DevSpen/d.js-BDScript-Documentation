# $serverNSFWLevel
Returns the NSFW level of a server.

### What are the available server NSFW levels?
[PAGE:Server NSFW Types]()

## Usage
```
$serverNSFWLevel[(optional) guildID]
```

### Breakdown
`guildID` - The server to get the data from. If this field is not inputted, the current server is used.

## Example
```js
bot.command({
    type: "command",
    name: "server-nsfw",
    code: `This server's NSFW level is: $serverNSFWLevel`
})
```
