# $botCount
Returns the total number of bots in a server.

## Usage
```
$botCount[(optional) guildID]
```
> If no 'guildID' is provided, it returns the bot count for the current server.

## Example
```js
bot.command({
    type: "command",
    name: "bot-count",
    code: `There are $botCount bots in this server!`
})
```
