# $getAllServerVarIDs
Returns all the server IDs that have atleast one variable value assigned to them in the database.

## Usage
```
$getAllServerVarIDs[(optional) separator]
```

### Breakdown
`separator` - The separator between each ID.

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `$getAllServerVarIDs
    $onlyForIDs[$botOwnerID;Only my owner can use that!]`
})
```
