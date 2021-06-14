# $userPerms
Returns the permissions for the provided user.

## Usage
```
$userPerms[guildID;userID;(optional) ifAdmin (yes/no)]
```

### Breakdown
`guildID` - The server to check the users permissions in. Use `$guildID` for the current server.

`userID` - The user to get the permissions for.

`ifAdmin` - What to return if the user has the administrator permission. Default is `no`.
  - `yes` = Only 'Administrator' will be returned, if the user has administrator.
  - `no` = All permissions will still appear (including administrator), even if the user has administrator.

## Example
```js
bot.command({
    type: "command",
    name: "permissions",
    code: `$userTag[$mentioned[1;yes]]'s permissions: $userPerms[$guildID;$mentioned[1;yes];yes]`
})
```
