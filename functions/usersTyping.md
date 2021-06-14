# $usersTyping
Returns a list of users that are typing in a channel.

## Usage
```
$usersTyping[channelID;(optional) option;(optional) separator]
```

### Breakdown
`channelID` - The channel to get the data from.

`option` - The data to return for the users typing. Default is option is `username`. Valid options: `mention`, `id`, `username`, `count`.

`separator` - The separator between user-data pieces, default is `, `.

## Example
```js
bot.command({
    type: "command",
    name: "typing",
    code: `Typing Users: $usersTyping[$channelID]`
})
```
