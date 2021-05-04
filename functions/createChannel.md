# $createChannel
Creates a channel in a guild, you can leave empty not needed fields.

## Usage
```$createChannel[guild ID;name;type;category ID;position;nsfw (yes/no);topic message;reason;returnChannelID (yes/no)]```

### Breakdown

Required Fiels:

`guild ID` - The guild to create this channel in.

`name` - The name for the channel.


Optional Fields:

`type` - The type for the channel. Default is `text`.

`category ID` - The category where this channel will be located at.

`position` - The position under the category.

`nsfw` - Whether this channel should be NSFW.

`topic message` - The topic for the channel.

`returnChannelID` - Whether to return the created channel's ID. Default is `no`.

## Example
```
bot.command({
    type: "command",
    name: "channel-create",
    code: `$createChannel[$guildID;general]
    Channel created.
    `
})
```

With optional fields,
```
bot.command({
    type: 'command',
    name: 'create-channel',
    code: `$createChannel[$guildID;general;text;$categoryID;1;no;This is the public channel.;no]
    Channel created.
})
