# $findMember
Finds a member of a server. Unlike `$findUser`, because its per-server; not global.

## Usage
```
$findMember[guildID;user;returnAuthorID (yes/no)]
```

### Breakdown
`guildID` - The server to find the user in.

`user` - The ID/mention/username of the user.

`returnAuthorID` - Whether to return the author's ID if no user is found or not.

## Example
```js
bot.command({
    type: "command", 
    name: "member-search", 
    code: `$onlyIf[$message!=;Please provided a user!]
    $replaceText[$findMember[$guildID;$message;yes];$authorID;User not found!;1]`
})
```
