# $getBotInvite
Gets the bot's invite URL.

## Usage
```
$getBotInvite[(optional) permissions]
```

### Breakdown
`permissions` - The [permissions](https://djs-bdscript.gitbook.io/docs/begin/permissions) to grant for the bot invite. Separate permissions using `;`.

## Example
```js
  bot.command({
    type: "command", 
    name: "invite", 
    code: `You can invite me here: $getBotInvite`
})
```
