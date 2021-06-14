# $userDevices
Returns what device(s) the user is on.

### What are the possible responses?

[Page:User Devices](https://djs-bdscript.gitbook.io/docs/properties/device-types)

## Usage
```
$userDevices[userID;(optional) separator]
```

### Breakdown
`userID` - The user to get the device for.

`separator` - The separator between devices (if multiple). Default is `, `.

## Example
```js
bot.command({
    type: "command",
    name: "device",
    code: `$userTag[$mentioned[1;yes]]'s device: $userDevices[$mentioned[1;yes]]`
})
```
