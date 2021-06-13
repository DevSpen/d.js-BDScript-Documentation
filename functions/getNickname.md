# $getNickname
Returns a user’s nickname. If the user doesn't have a nickname, nothing is returned. (Unlike `$nickname`, which returns the user's username if they don't have a nickname.)

## Usage
```
$getNickname[guildID;userID]
```
> If all fields are left empty, the bot returns the nickname of the author in the current server.

### Breakdown
`guildID` - The server to get the user's nickname from.

`userID` - The user to get the nickname for.

## Example
```js
bot.command({
    type: "command",
    name: "my-nick",
    code: `<@$authorID>'s nickname: $getNickname`
})
```
