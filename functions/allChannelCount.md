# $allChannelCount
Returns the total numbers of channels from all servers that the bot is in.

## Usage
```
$allChannelCount
```

## Example
```js
bot.command({
    type: "command",
    name: "total-channels",
    code: `There are $allChannelCount channels total!`
})
```
