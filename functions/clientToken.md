# $clientToken
Returns the bot's token.

[WarningMsg] This should be kept private to the developer. Use functions like `$sendDM` and `$onlyForIDs`. Example can be found below.


## Usage
```
$clientToken
```

## Example
```js
bot.command({
 type: "command"
 name: "token",
 code: `$sendDM[$botOwnerID;Here's my token: $clientToken;no]
 $onlyForIDs[$botOwnerID;You are not my owner, so you can't use that!]`
 })
 ```
