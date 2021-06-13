# $isServerDeafened
Returns whether or not a user is server-deafened.

> 'true' means the user is server-deafened, 'false' means the user isn't.

> Server-deafened is when the user is forced deafened in VC by a server admin/staff.

## Usage
```
$isServerDeafened[guildID;userID]
```
> You can also use just `$isServerDeafened` without any fields, to return data from the author in the current server.

## Breakdown
`guildID` - The server to get the data from.

`userID` - The user to get the data for.
