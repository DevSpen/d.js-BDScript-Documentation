# $songInfo
Returns info on a song added to the queue.

## Usage
```
$songInfo[guildID;option;songIndex]
```

### Breakdown
`guildID` - The server to get the queue from.

`option` - The data to get. [(see available properties)](https://djs-bdscript.gitbook.io/docs/properties/song-properties)

`songIndex` - The song to return info for, `1` stands for the song that is currently being played.

## Example
```js
bot.command({
    type: "command",
    name: "song-url",
    code: `Here's the link to the song that you are listening to: $songInfo[$guildID;url;1]`
})
```
