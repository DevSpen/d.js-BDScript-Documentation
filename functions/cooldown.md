# $cooldown
Sets a Command Cooldown.


## Usage
`$cooldown[time;errormsg]`


### Breakdown
`time` - The time of the Command Cooldown.
`errormsg` - The Error Message if the Cooldown is still ongoing.


## Exampe
```bot.command({
 type: "command",
 name: "cooldown"
 code: `Hi! This is just an example.
 $cooldown[5s;Error! You can use this command again at the next 5seconds.]`
 })````
