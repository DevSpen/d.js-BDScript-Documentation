# $serverCount
Returns how many servers the bot is in.

## Usage
```
$serverCount
```

## Example
```js
bot.command({
    type: "command",
    name: "servers",
    code: `I have currently in $serverCount servers!`
})
```
