# $clientDestory
Disconnects the client from Discord.

## Usage
```
$clientDestroy
```
> You shouldn't put this in any public commands, use it with care.

## Example
```js
bot.command({
    type: "command",
    name: "disconnect",
    code: `$clientDestroy
    $onlyForIDs[$botOwnerID;You aren't my owner so you can't use that command!]`
})
```
