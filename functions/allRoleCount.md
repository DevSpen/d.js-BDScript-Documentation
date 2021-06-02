# $allRoleCount
Returns the total numbers of roles from every server the bot is in.

## Usage
```
$allRoleCount
```

## Example
```js
bot.command({
    type: "command",
    name: "all-roles",
    code: `There are $allRoleCount roles from all my servers combined.`
})
```
