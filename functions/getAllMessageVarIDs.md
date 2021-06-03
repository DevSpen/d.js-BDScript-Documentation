# $getAllMessageVarIDs
Returns all the message IDs that have at least one variable value assigned in the database.

## Usage
```
$getAllMessageVarIDs[(optional) separator]
```

### Breakdown
`separator` - The separator between each ID.

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `$getAllMessageVarIDs
    $onlyForIDs[$botOwnerID;Only my owner can use that!]`
})
```
