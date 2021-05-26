# Intro
```js
bot.command({
    type: "command", // Put the command type here
    // Add all needed fields below.
})
```

## Example
```js
bot.command({
    type: "command", 
    name: "something", 
    code: `nice!`
})
// Tip: Except for the last field (in this case 'code'), you should include a comma (,) after the field.
```

# Types
## command
A standard command.
`name` - The name (trigger) of the command. This property is required. 
`code` - The code to run when the command is triggered. This property is required. 
`aliases` - View aliases guide. This property is not required.

## deleteCommand
Triggered when a message is deleted.
`channel` - The channel the message is posted in. This property is required.
`code` - The code to run. This property is required.

## reactionAddCommand
Triggered when a reaction is added to a message.
`channel` - The channel the message is posted in. This property is required. 
`code` - The code to run. This property is required.

## reactionRemoveCommand
Triggered when a reaction is removed from a message.
`channel` - The channel the message is posted in. This property is required. 
`code` - The code to run. This property is required.

## updateCommand
Triggered when a message gets edited.
`channel` - The channel to post the message in.This property is required. 
`code` - This property is required.

## readyCommand
Triggered when the bot goes online.
`channel` - This property is required. 
`code` - This property is required.

## spaceCommand
Replies to every user's message. Use this wisely!
`name` - This property is not required. 
`code` - This property is required.

## joinCommand
Triggered when a user joins the server.
`channel` - This property is required. 
`code` - This property is required.

## leaveCommand
Triggered when a user leave the server.
`channel` - This property is required. 
`code` - This property is required.
