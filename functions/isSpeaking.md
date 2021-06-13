# $isSpeaking
Returns whether or not the user is currently speaking. A boolean if the information is available (aka the bot is connected to any voice channel in the server), otherwise this is null.
> 'true' means the user is speaking, 'false' means the user isn't.

## Usage
```
$isSpeaking[guildID;userID]
```
> You can also use `$isSpeaking` without any fields, to get the data from the author and current server.

### Breakdown
`guildID` - The server to get the data from.

`userID` - The user to get the data for.

## Example
```js
  bot.command({
    type: "command", 
    name: "speaking", 
    code: `Are you speaking?: $isSpeaking`
})
```
