# $authorAvatar
Returns the author's avatar.

## Usage
```$authorAvatar```

### Example
```js
bot.command({
    type: "command",
    name: "my-avatar",
    code: `$title[$username's Avatar]
    $image[$authorAvatar]`
})
```
