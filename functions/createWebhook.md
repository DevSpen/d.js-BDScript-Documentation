# $createWebhook
Creates a webhook and returns its URL.

## Usage
```
$createWebhook[channelID;name;avatarURL]
```

### Breakdown
`channelID` - The channel to create the webhook in.

`name` - The display name of the webhook.

`avatarURL` - The avatar of the webhook.

## Example
```js
bot.command({
    type: "command",
    name: "webhook",
    code: `$createWebhook[837825243376648232;Cool Webhook;$authorAvatar]
    $onlyIf[$hasPerm[$guildID;$authorID;managewebhooks]==true;Missing permissions. You can't use that!]`
})
```
