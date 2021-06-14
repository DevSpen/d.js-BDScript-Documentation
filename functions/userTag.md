# $userTag
Returns the user's tag (User#0000).

## Usage
```
$userTag[(optional) userID]
```

### Breakdown
`userID` - The user to get the tag for.

## Example
```js
bot.command({
    type: "command",
    name: "tag",
    code: `<@$mentioned[1;yes]>'s tag is $userTag[$mentioned[1;yes]]`
})
```
