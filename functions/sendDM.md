# $sendDM
Sends a direct message to the provided user.

## Usage
```
$sendDM[userID;message;(optional) returnMessageID (yes/no)]
```

### Breakdown
`userID` - The user to send the DM message to.

`message` - The message that the user gets DM'd.

`returnMessageID` - Whether or not to return the direct message ID. Default is `no`.

## Example
```js
bot.command({
    type: "command",
    name: "hi",
    code: `$sendDM[$authorID;hi]`
})
```
