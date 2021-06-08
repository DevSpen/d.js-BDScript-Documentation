# $getUserReactions
Returns user data from a emoji reaction of a message

## Usage 
`$getUserReactions[channelID;messageID;emoji;option;separator]`

### Breakdown 
`channelID` - ID of the channel where the message was sent 
`messageID` - ID of the message with the reaction's data you are going to be pulling
`emoji` - The emoji of which data is being pulled 
`option` - The data type being pulled. 
`separator` - Separator of the data 

[InfoMsg] Options can be data like `id`, `username` , `mention` , `count` etc..

## Example
```
bot.command({
    type:"command"
    name:"test"
    code:`users who reacted to this message are 
$getUserReactions[837405027911991366;850432691069517824;❤️;mention;|]
`
})
```
[WarningMsg] To pull data of a custom or nitro emote, it's recommended to use the unicode of the emote like this <:name:emojiID:> or <a:name:emojiID:> for animated custom emotes.

