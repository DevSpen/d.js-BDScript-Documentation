# $getGlobalUserVar
Returns a global-user variable value.

## Usage
```
$getGlobalUserVar[variableName;(optional) userID]
```

### Breakdown
`variableName` - The name of the variable to get.

`userID` - The user to get the variable value for. If field isn't inputted, then the author is used.

## Example
```js
bot.command({
    type: "command",
    name: "balance",
    code: `You have $getGlobalUserVar[Money] coins.`
})
```
