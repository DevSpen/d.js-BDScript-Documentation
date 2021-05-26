# $channelCooldown
Sets a channel cooldown. After the command is executed, no one can use the command in the current channel until the `duration` is up. If the duration is still ongoing, the `error message` will appear.

## Usage
```$channelCooldown[duration;error message]```

### Breakdown
`duration` - How long the cooldown delay is.

`error message` - The code to execute when the duration is ongoing.

### Example Usage
```$channelCooldown[30s;This command is on channel cooldown! Please wait $data[time] to use that command again!]```

## Using $data
You can use `$data` to get how much time is left before the cooldown expires. Simply, put `$data[time]`.
> `$data[time]` can only be used in the `error message` field.
