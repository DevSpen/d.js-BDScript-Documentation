# $sendCrosspostMessage
Sends the same message in multiple channels.

[WarningMsg] Use this function wisely! 

## Usage
```
$sendCrosspostMessage[channels;message]
```

### Breakdown
`channels` - The channels to send the 'message' in. Separate IDs using `;`.

`message` - The message to send in the 'channels'.

## Example
```js
bot.command({
    type: "command",
    name: "nya",
    code: `$sendCrosspostMessage[837439473129357413;837405905137827881;nya]`
})
```
