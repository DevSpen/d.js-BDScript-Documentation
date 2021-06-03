# $getAllGlobalUserVarIDs
Returns the IDs of all the users that have atleast one global user variable value assigned in the database.

## Usage
```
$getAllGlobalUserVarIDs[(optional) separator]
```

### Breakdown
`separator` - The separator between each ID (e.g `,`)

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `$getAllGlobalUserVarIDs
    $onlyForIDs[$botOwnerID;Only my owner can use that!]`
})
```
