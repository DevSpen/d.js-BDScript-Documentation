# $getInviteInfo
Gets info about a invite code.

## Usage
```
$getInviteInfo[code;data]
```

### Breakdown
`code` - The invite code to get info about.

`data` - The info to get about the invite. [(see invite properties)](https://djs-bdscript.gitbook.io/docs/properties/invite-properties)
  
## Example
```js
  bot.command({
    type: "command", 
    name: "example", 
    code: `There are: $getInviteInfo[uyJjEzQH;uses] uses of the main invite.`
})
```

