# $addMessageReactions
Adds reaction(s) to a message.

## Usage
```$addMessageReactions[channelID;messageID;emoji1;(optional) emoji2;(optional) etc]```

### Breakdown
`channelID` - The channel ID of the message the bot will react to.

`messageID` - The message ID of the message the bot will react to.

`emoji1` - The emoji the bot reacts to the message with. Accepts unicode emojis and emoji ids.

`emoji2` - The second emoji the bot reacts with. Optional.

`etc` - You can react with up to 20 emojis. Additional emoji fields are optional.

## Example
```
bot.command({
    type: "command",
    name: "clown",
    code: `$addMessageReactions[$channelID;$messageID;🤡] // This would react to the author's message.
    $username is a clown`
})
```
