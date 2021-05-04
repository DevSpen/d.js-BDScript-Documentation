# $clientID
Returns the logged client's ID.

## Usage
```$clientID```

## Example
```
bot.command({
    type: "command",
    name: "check-condition",
    code: `My ID is $clientID.
    `
})
```
