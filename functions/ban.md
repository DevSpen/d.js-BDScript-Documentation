# $ban
Bans a user from a guild.

## Usage
```$ban[guildID;userID;reason;days]```

### Breakdown
`guildID` - The server that the user gets banned from. Use `$guildID` for the current server.

`userID` - The user who is being banned.

`reason` - The reason why the user is getting banned. (for audit log)

`days` - Messages to delete that are newer to these days. Put `0` for none.

## Example
```
bot.command({
    type: "command",
    name: "ban",
    code: `$ban[$guildID;$mentioned[1];$replaceText[$message;$message[1];;1];0]`
})
```
