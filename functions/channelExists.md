***$channelExists***

Checks if the given channel ID exists in the Server.

***Usage***

`$channelExists[channel_id]`

If the given channel ID exists, it wi return `true`. And if the given channel ID isn't existed, it will return false.

***Example***

```bot.command({
   type: "command"
   name: "channelexists",
   code: "$channelExists[$message[1]]"
   })```
