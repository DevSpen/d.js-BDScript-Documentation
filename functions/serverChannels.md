# $serverChannels
Returns all the channels in a server.

## Usage
```
$serverChannels[(optional) guildID;(optional) option;(optional) separator;(optional) filters]
```

### Breakdown
`guildID` - The server to get the channels for. Use the current server by default.

`option` - The channel property to return for each channel [(see channel properties)](https://djs-bdscript.gitbook.io/docs/properties/channel-properties). Uses `name` by default.

`separator` - The separator between each channel property. Default is `, `.

`filters` - Filter server channels by channel types [(see channel types)](https://djs-bdscript.gitbook.io/docs/properties/channel-types). Separate IDs using `;`. Default is none.

## Example
```js
bot.command({
    type: "command",
    name: "channels",
    code: `Server Channel IDs: $serverChannels[$guildID;id]`
})
```
