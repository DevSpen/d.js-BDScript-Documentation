# $getUserVar
Returns a local-user variable value.

## Usage
```
$getUserVar[variableName;(optional) userID;(optional) guildID]
```

### Breakdown
`variableName` - The name of the variable to get.

`userID` - The user to get the variable value for. If no user is provided, the author is used.

`guildID` - The server to get the variable value from. If no server is provided, the current server is used.

## Example
```js
bot.command({
    type: "command",
    name: "balance",
    code: `<@$mentioned[1;yes]> has $getUserVar[Money;$mentioned[1;yes]] coins.`
})
```
