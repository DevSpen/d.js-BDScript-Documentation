# $isStreaming
Returns whether or not a user is streaming in VC using Go Live.
> 'true' means the user is streaming, 'false' means the user isn't.

## Usage
```
$isStreaming[guildID;userID]
```
> You can also use `$isStreaming` without any fields, to get the data from the author and current server.

### Breakdown
`guildID` - The server to get the data from.

`userID` - The user to get the data for.

## Example
```js
  bot.command({
    type: "command", 
    name: "speaking", 
    code: `Is $userTag[$mentioned[1;yes]] streaming?: $isStreaming[$mentioned[1;yes]]`
})
```
