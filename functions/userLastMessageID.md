# $userLastMessageID
Returns the user's latest message ID.

## Usage
```
$userLastMessageID[(optional) userID]
```

### Breakdown
`userID` - The user to get the latest messageID for. If this field is not provided, the author's latest messageID is returned.

## Example
```js
bot.command({
    type: "command",
    name: "latest-message",
    code: `Your latest messageID: $userLastMessageID`
})
````
