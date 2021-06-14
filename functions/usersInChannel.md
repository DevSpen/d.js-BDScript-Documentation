# $usersInChannel
Returns a list of users that are currently in the provided voice channel.

## Usage
```
$usersInChannel[voiceChannelID;option;separator]
```

### Breakdown
`voiceChannelID` - The voice channel to get the users from.

`option` - The data to return about the users, default is `username`. Valid options: `mention`, `username`, `id`, `discriminator` `count`, etc.

`separator` - The separator between each user-data piece, default is `, `.

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `There are $usersInChannel[389478234783474749;count] users in the music VC!`
})
```
