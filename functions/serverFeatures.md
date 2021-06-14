# $serverFeatures
Returns the server's features.

## Usage
```
$serverFeatures[(optional) guildID;(optional) separator]
```

### Breakdown
`guildID` - The server to get the features from. Uses the current server, if none is provided.

`separator` - The separator between features. Default is a comma (`, `).

### Possible Features
- Animated Icon
- Banner
- Commerce
- Community
- Discoverable
- Featureable
- Invite Splash
- News
- Partnered
- Relay Enabled
- Vanity URL
- Verified
- VIP Regions
- Welcome Screen Enabled

## Example
```js
bot.command({
    type: "command",
    name: "features",
    code: `Features: $serverFeatures`
})
```
