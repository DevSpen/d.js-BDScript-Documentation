# $isSystemMessage
Whether or not this message was sent by Discord, not a actual user (e.g pin notifications).
> 'true' means the author's message was a system message, 'false' means it wasn't.

## Usage
```
$isSystemMessage
```

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `Is System Message: $isSystemMessage`
})
```
