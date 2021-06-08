## [GET:TITLE]
Callbacks are commands that get executed when a certain Discord event happens. These are very useful for logging!

## Setting Up Callbacks
### Adding Events
All callbacks require the event to be added.

Simply use `bot.addEvent("event")`, example:
[InfoMsg] You only need to add the event once!

```js
bot.addEvent("onJoined")
// This example adds the onJoined event.
````

### All Available Events
- onJoined 
- onReady 
- onReactionAdd 
- onReactionRemove 
- onLeave 
- onMessage 
- onMessageUpdate 
- onMessageDelete

## Creating Callback Commands
All callback commands require different fields (check command-types for more info). 

### Types List
*(click on the type for more info)*
- joinCommand 
- leaveCommand 
- deleteCommand 
- reactionAddCommand 
- reactionRemoveCommand 
- updateCommand 
- readyCommand 
- spaceCommand

### Callback Guides
[GET:URLS]("import.md")

### Using Server Variables
You can use server-variables for the 'channel' when making callbacks. This is because almost all callbacks are global. 

### Example
```js
bot.command({
    type: "joinCommand", // This example is a onJoined command.
    channel: "$getServerVar[WelcomeChannel]", // Will get the channel ID to send the in from the variable.
    code: `<@$authorID> just joined the server!` // This is the message that sends.
})
```
