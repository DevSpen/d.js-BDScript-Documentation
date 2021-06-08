# $getUserReactions
Returns user data from a emoji reaction of a message.

## Usage 
`$getUserReactions[channelID;messageID;emoji;option;separator]`

### Breakdown 
`channelID` - The channel that the message belongs to.

`messageID` - The ID of the message with the reaction's data to get.

`emoji` - The emoji to get the data for.

`option` - The data type being pulled. For example, `id`, `username` , `mention` , `count` etc.

`separator` - Separator between data values.


## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `$getUserReactions[837405027911991366;850432691069517824;❤️;id;|]`
})
```
[InfoMsg] To get data from a custom emoji, it's recommended to use the ID of the emote, like: `<:name:emojiID:>` (for regular) or `<a:name:emojiID:>` (for animated).

