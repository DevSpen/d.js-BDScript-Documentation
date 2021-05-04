# $createEmoji
Creates a Emoji in a guild.

## Usage
```$createEmoji[guild ID;name;url;reason;returnEmoji (yes/no);role]```

### Breakdown

Required Fiels:

`guild ID` - The guild to create the emoji on.

`name` - The name for the emoji.

`url` - The url for the emoji.


Optional Fields:

`reason` - The reason for creating this emoji.

`returnEmoji` - Whether to return the created emoji. Default is `yes`.

`roles` - Role to whitelist. Can be multiple by separating `;`.

## Example
```
bot.command({
    type: "command",
    name: "emoji-create",
    code: `New Emoji has been created.
    $createEmoji[$guildID;laugh;https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/320/google/274/rolling-on-the-floor-laughing_1f923.png].
    `
})
```

With optional fields,
```
bot.command({
    type: 'command',
    name: 'create-channel',
    code: `New Emoji $createEmoji[$guildID;laugh;https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/320/google/274/rolling-on-the-floor-laughing_1f923.png;New laugh emoji;yes;$guildID]
})
