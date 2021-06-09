# $isManageable
Whether the bot is above a user in the hierarchy, according to role position and server ownership. In short, returns if the bot can manage the user.

> 'true' means the bot can manage the user, 'false' means it can't.

## Usages
There are two usages of the `$isManageable` function.

### Usage #1
```
$isManageable
```
> Returns whether or not the author is manageable, in the current server.

### Usage #1
```
$isManageable[guildID;userID]
```
> Returns whether or not the inputted user is manageanble, in the provided server.

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `Can I manage you?: $isManageable`
})
```
