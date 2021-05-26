# $channelCategoryID
Gets the ID of the category a channel belongs to.

## Usages
- There are two usages to the `$channelCategoryID` command.

### Usage #1
`$channelCategoryID` - Gets the ID of the category; that the current channel belongs to.

### Usage #2
`$channelCategoryID[channelID]` - Gets the ID of the category; the channel provided belongs to.

## Example
```js
bot.command({
    type: "command",
    name: "category",
    code: `Here's the category ID that this channel is in: $channelCategoryID`
})
```
