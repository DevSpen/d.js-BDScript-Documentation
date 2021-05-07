# $serverIcon
Returns a server's icon.

## Usage #1
• `$serverIcon` with options. Returns a server's icon with the provided data.

```$serverIcon[guildID;size;animated (yes/no)]```

### Breakdown
`guildID` - The server to retrieve the icon from. Use `$guildID` for current server.

`size` - The size for the icon. (e.g 1024, 2048, 4096)

`animated` - Whether the icon should be animated if its a GIF.

## Usage #2
• `$serverIcon` without options. Returns the current server's icon.

```$serverIcon```

## Example
```
bot.command({
    type: "command",
    name: "server-icon",
    code: `$image[$serverIcon[$guildID;4096;yes]]`
})
```
