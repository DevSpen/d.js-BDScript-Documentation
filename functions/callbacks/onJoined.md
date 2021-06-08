# onJoined
Triggered when a user joins a server.

Add The Event: `bot.addEvent("onJoined")`

Type: `joinCommand`

## Base Code
```js
bot.command({
    type: "joinCommand", // onJoined type.
    channel: "channelID", // The channel which the message gets sent in.
    code: `code` // The code to run when someone joins.
})
```

## Example
```js
bot.command({
    type: "joinCommand",
    channel: "39459438494840494",
    code: `<@$authorID> just joined the server!`
})
```

[WarningMsg] This requires members intent enabled!

[InfoMsg] onJoined triggers for all servers that your bot is in. You can prevent this by using server variables. [learn-more]()
