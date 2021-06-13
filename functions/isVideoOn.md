# $isVideoOn
Returns whether or not a user has their video enabled in VC.
> 'true' means the user's video is on, 'false' means its off.

## Usage
```
$isVideoOn[(optional) guildID;(optional) userID]
```

### Breakdown
`guildID` - The server to get the data from. Uses the current server if none is provided.

`userID` - The user to get the data for. Uses author if none is provided.


## Example
```js
  bot.command({
    type: "command", 
    name: "video", 
    code: `Is your video on?: $isVideoOn`
})
```
