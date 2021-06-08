# $songInfo
Returns info on a song added to the queue.

## Usage
```
$songInfo[guildID;option;songIndex]
```

### Breakdown
`guildID` - The server to get the queue from.

`option` - The data to get. (refer to the Available Options section)

`songIndex` - The song to return info for, `1` stands for the song that is currently being played.

## Available Options
- `userID` - The ID of the user who added this song to the queue.
- `username` - The username of the user who added this song to the queue.
- `thumbnail` - The thumbnail image of the song.
- `title` - The title of the song.
- `author` - The author of the song.
- `duration` - How long the song is.
- `userTag` - Gets a user's username in the proper format (User#0000)
- `url` - The URL of the song.

## Example
```js
bot.command({
    type: "command",
    name: "song-url",
    code: `Here's the link to the song that you are listening to: $songInfo[$guildID;url;1]`
})
```
