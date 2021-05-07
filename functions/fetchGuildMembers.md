# $fetchGuildMembers
Fetches all the members from the given server. Requires 'guild members' intent.

## Usage
```$fetchGuildMembers[guild ID (optional)]```

### Breakdown

`guild ID` - The server to fetch the members from.


## Example
```
bot.command({
    type: "command",
    name: "members",
    code: `
    Members: $fetchGuildMembers //The result may not be stable if the server has more than hundred members.
    `
})
```
