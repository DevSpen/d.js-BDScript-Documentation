# $channelNSFW
Returns whether a channel is NSFW or not.
> `true` means the channel is NSFW, `false` means it isn't.

## Usages
- There are two usages for the `$channelNSFW` command.

### Usage #1
`$channelNSFW` - Returns whether the current channel is NSFW or not.

### Usage #2
`$channelNSFW[channelID]` - Returns whether the channel provided is NSFW  or not.

## $channelNSFW Limiter
`$onlyIf[$channelNSFW==true;error message.]` - Prevents the command being executed outside of NSFW channels. 
> Tip: Use this in any NSFW commands your bot has!

## Example
```js
bot.command({
    type: "command",
    name: "nsfw",
    code: `😳
    $onlyIf[$channelNSFW==true;This command can only been used in NSFW channels!]`
})
```

