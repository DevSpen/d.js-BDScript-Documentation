# $getServerInvite
Returns the server invite URL.

## Usage
```
$getServerInvite[(optional) guildID]
```

### Breakdown
`guildID` - The server to generate the invite for. If this field is not inputted, the current server is used.

## Example
```js
bot.command({
    type: "command",
    name: "server-invite",
    code: `Server Invite: $getServerInvite`
})
```
