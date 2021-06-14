# $userStatus
Gets a user's status.

## Usage
```
$userStatus[(optional) userID]
```

### Breakdown
`userID` - The user to get the status for. If no user is provided, the author's status is returned.

### Possible Responses
- `online`
- `dnd` (do-not-disturb)
- `idle`
- `offline`

## Example
```js
bot.command({
    type: "command",
    name: "status",
    code: `Your status is: $userStatus`
})
```

