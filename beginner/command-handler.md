# Command-Handler
Command Handler is the Handler that can read the given Path as "commands".


## Usage
`bot.manager.load(path)`


### Breakdown
`path` - The Folder that you want to read.


## Example
```const bot = new bdjs({
    token: "token here", //bot token
    prefix: "prefix" //accepts an array of prefixes too 
})

bot.manager.load("./commands/")

bot.login()
bot.addEvent("onMessage")
bot.command({
    type: "command", //the command type
    name: "say", //command trigger
    code: "$message"
})````

You can now do:
```module.exports = ({
 type: "command",
 name: "ping",
 code: `$pingms`
})```

You can also do "$updateCommands" to update your Commands without restarting your Host.



Note: You need to upgrade the package my changing the version on "package.json" into latest one! Latest Version: `4.0.1`
