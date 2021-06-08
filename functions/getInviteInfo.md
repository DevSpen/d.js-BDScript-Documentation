# $getInviteInfo
Gets info about a invite code.

## Usage
```
$getInviteInfo[code;data]
```

### Breakdown
`code` - The invite code to get info about.

`data` - The info to get about the invite.

## Data Properties 
- `uses`
  - How many times the invite has been used.

- `userID`
  - The person that created the invite.

- `guildID`
  - The server that the invite belongs to.

- `channelID`
  - The channel this invite was created in.

- `url`
  - Full link of the invite.

- `expiresAt`
  - The invite expiration date.

- `expiresTimestamp`
  - The invite expiration date in milliseconds.
   
- `maxUses`
  - The max uses for this invite.

- `memberCount`
  - The member count of the server, that the invite is from.
      
- `presenceCount`
  - The presence count of the server, that the invite is from.
 
- `maxAge`
  - The duration of the invite, 0 = forever.
      
- `temporary`
  - Whether or not the invite is temporary.

- `deletable`
  - Whether this invite is deletable by the bot.
  
## Example
```js
  bot.command({
    type: "command", 
    name: "example", 
    code: `There are: $getInviteInfo[uyJjEzQH;uses] uses of the main invite.`
})
```

