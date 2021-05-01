# $addField
Adds a field to the embed.

## Usage
```$addField[name;value;(optional) inline (yes/no)]```

### Breakdown
`name` - The "name" of the field.

`value` - The "value" of the field.

`inline` -  Sets if fields are inlined. yes = inline. no = not inlined. The default is "no".

## Example
```
bot.command({
    type: "command",
    name: "say",
    code: `$addField[Hi!;I'm called $username[$clientID].;yes]
$addField[Wow!;You have a lovely name, $username!;yes]`
})
```

#### Notices
[Info Msg] You can only use 25 fields per message.
