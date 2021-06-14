# $usersBanned
Returns all banned users from the server.

## Usage
```
$usersBanned[guildID;(optional) option;(optional) separator]
```

### Breakdown
`guildID` - The server to get the banned users for.

`option` - The data to return about the banned users, default is `username`. Valid options: `mention`, `username`, `id`, `count`, `discriminator`, etc. 

`separator` - The separator between each user-data piece, default is `, `.

## Example
```js
bot.command({
    type: "command",
    name: "banned",
    code: `Banned Users: $usersBanned[$guildID;id]`
})
```
