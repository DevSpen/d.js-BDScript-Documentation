# $exec
Executes a command in the powershell.

## Usage
```$exec[command]```

### Breakdown

`command` - The command line to execute.


## Example
```
bot.command({
    type: "command",
    name: "execute",
    code: `
    $exec[npm -v] //Returns the current npm version.
    `
})
```
