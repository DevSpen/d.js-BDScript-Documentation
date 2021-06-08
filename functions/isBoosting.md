# $isBoosting
Returns whether or not a user is boosting.

> 'true' means the user is boosting, 'false' the user isn't boosting.

## Usage
```
$isBoosting[guildID;userID]
```

### Breakdown
`guildID` - The server to use when checking if the user is boosting. Use `$guildID` for the current server.

`userID` - The user to check.

> You can also just use `$isBoosting` without any fields, this will return the data for the author in the current server.

## Example
```js
bot.command({
    type: "command",
    name: "is-boosting",
    code: `Are You Boosting? $isBoosting`
})
```
