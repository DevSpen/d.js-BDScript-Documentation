# $userAvatar
Returns a user's avatar URL.

## Usage
```
$userAvatar[userID;(optional) size;(optional) dynamic (yes/no)]
```

### Breakdown
`userID` - The user to get the avatar for.

`size` - The wanted size of the avatar [(see image size properties)](https://djs-bdscript.gitbook.io/docs/properties/image-size-properties)

`dynamic` - Whether to display the avatar as a GIF, if its animated or not. Default is `yes`.

## Example
```js
bot.command({
    type: "command",
    name: "avatar",
    code: `$title[1;$userTag[$mentioned[1;yes]]'s Avatar]
    $image[1;$userAvatar[$mentioned[1;yes];4096;yes]]`
})
```
