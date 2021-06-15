# $serverCooldown
Sets a server cooldown. After the command is used, no one in the server will be able to run the command until the `duration` is up.

## Usage
```
$serverCooldown[duration;errorMessage]
```

### Breakdown
`duration` - The duration of the cooldown.

`errorMessage` - The error that is returned if the 'duration' is still ongoing. You can use `$data[time]` in this field, to get how much time is left on the cooldown.

## Example
```js
bot.command({
    type: "command",
    name: "ping",
    code: `$serverCooldown[10s;Someone has already used this command recently! Please wait $data[time].]
    Pong! $ping ms`
})
```
