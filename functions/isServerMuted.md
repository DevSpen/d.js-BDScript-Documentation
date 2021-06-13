# $isServerMuted
Returns whether or not a user is server-muted.
> 'true' means the user is server-muted, 'false' means the user isn't.

> Server-muted is when the user is forced muted in VC by a server admin/staff.

## Usage
```
$isServerMuted[guildID;userID]
```
> You can also use just `$isServerMuted` without any fields, to return data from the author in the current server.

### Breakdown
`guildID` - The server to get the data from.

`userID` - The user to get the data for.
