# $kick
Kicks a user from the provided server.

## Usage
```$kick[guildID;userID;reason]```

### Breakdown
`guildID` - The server that the user gets kicked from. Use `$guildID` for the current server.
`userID` - The user who is being kicked.
`reason` - The reason why the user is getting kicked (for the audit log).

## Example
```bot.command({
    type: "command",
    name: "kick",
    code: `$kick[$guildID;$mentioned[1];$replaceText[$message;$message[1];;1]]` // kicks the mentioned user.
})```
