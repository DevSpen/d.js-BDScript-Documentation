# onLeave
Triggered when a user leaves a server.

Add The Event: `bot.addEvent("onLeave")`

Type: `leaveCommand`

## Base Code
```js
bot.command({
    type: "leaveCommand", // onLeave type.
    channel: "channelID", // The channel which the message gets sent in.
    code: `code` // The code to run when someone leaves.
})
```

## Example
```js
bot.command({
    type: "leaveCommand",
    channel: "39459438494840494",
    code: `<@$authorID> just left the server!`
})
```

[WarningMsg]This requires members intent enabled!

[InfoMsg] onLeave triggers for all servers. You can prevent this by using server variables. [learn-more]()
