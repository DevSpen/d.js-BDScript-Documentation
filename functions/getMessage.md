# $getMessage
Gets the specified components from a message.

## Usage
```
$getMessage[channelID;messageID;option;(optional) fieldIndex;(optional) embedIndex]
```

### Breakdown
`channelID` - The channel that the message belongs to.

`messageID` - The ID of the message to get.

`option` - What property to get. [(see message properties list)](https://djs-bdscript.gitbook.io/docs/properties/message-properties)

`fieldIndex` - When getting the content of a field name/value, you need to specify the index (e.g `1`, `2`, etc). This decides which field to return the data for. Default is `1`.

`embedIndex` - If multiple embeds are sent in the message, you can pick which to return. Default is `1`.

## Example
```js
bot.command({
    type: "command",
    name: "quote",
    code: `$description[1;$getMessage[$findChannel[$message[1]];$message[2];content]]
    $onlyIf[$argCount[$message]>=2;Please provide needed arguments! Usage: <prefix>quote (channel) (messageID)]`
})
```
