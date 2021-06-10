# $serverVanityCode
Returns a servers vanity code (if one exists).

> In order to get a vanity URL, the server needs to have 30 boosts, or be Discord partnered/verified. The vanity URL is set in the server settings.

## Usage
```
$serverVanityCode[(optional) guildID]
```

### Breakdown
`guildID` - The server to return the data for. If nothing is provided, it returns data for the current server.

## Example
```js
bot.command({
    type: "command", 
    name: "vanity-url", 
    code: `Our vanity URL is: discord.gg/$serverVanityCode`
})
```
