# $fetchGuildMembers
Fetches all the members from the given server. Requires members intent enabled in the [developer portal](https://discord.com/developers/applications).

## Usage
```$fetchGuildMembers[guild ID (optional)]```

### Breakdown
`guild ID` - The server to fetch the members from. If none is provided, it uses the current server.


## Example
```
bot.command({
    type: "command",
    name: "members",
    code: `Members: $fetchGuildMembers`
})
```
[Info Msg] The result may not be stable if the server has more than hundred members.
