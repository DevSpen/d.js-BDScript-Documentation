# $createEmoji
Creates a emoji.

## Usage
```$createEmoji[guild ID;name;url;reason;returnEmoji (yes/no);role]```

### Breakdown

#### Required Fields:

`guild ID` - The server to create the emoji in.

`name` - The name for the emoji.

`url` - The image URL for the emoji.


#### Optional Fields:

`reason` - The reason for creating this emoji (for the audit log)

`returnEmoji` - Whether to return the created emoji. Default is `yes`.

`roles` - Role to whitelist. Can be multiple by separating `;`.

## Example
```
bot.command({
    type: "command",
    name: "emoji-create",
    code: `New emoji has been created. 
    $createEmoji[$guildID;laugh;https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/320/google/274/rolling-on-the-floor-laughing_1f923.png].`
})
```

With optional fields,
```
bot.command({
    type: 'command',
    name: 'create-channel',
    code: `New emoji $createEmoji[$guildID;laugh;https://emojipedia-us.s3.dualstack.us-west-1.amazonaws.com/thumbs/320/google/274/rolling-on-the-floor-laughing_1f923.png;New laugh emoji;yes;$guildID]
})
