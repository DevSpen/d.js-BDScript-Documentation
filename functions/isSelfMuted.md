# $isSelfMuted
Returns whether or not a user is self-muted.

> 'true' means the user is self-muted, 'false' means the user isn't.

> Self-muted is when the user has muted themselves intentionally.

### Usage
```
$isSelfMuted[guildID;userID]
```
> You can also use just `$isSelfMuted` without any fields, to return data from the author in the current server.

### Breakdown
`guildID` - The server to get the data from.

`userID` - The user to get the data for.
