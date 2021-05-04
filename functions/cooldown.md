# $cooldown
Only allows the user to run the command if the cooldown is over.

## Usage
```$cooldown[time;error message]```


### Breakdown
`time` - How long a user has to wait to run the command again.
`error message` - The error message if the cooldown is still ongoing.


## Exampe
```
bot.command({
 type: "command",
 name: "cooldown"
 code: `Hi! This is just an example.
 $cooldown[5s;Error! You can use this command again in $data[time].]`
 })
 ```
[Info Msg] You can use `$data[time]` in cooldown error messages to tell how much time is left until the user can run the command.
