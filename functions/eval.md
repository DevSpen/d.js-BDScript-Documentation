# $eval
Evals d.js-BDScript code.

## Usage
```$eval[showOutput (message/yes/no);code]```

### Breakdown
`showOutput` - Whether to return the output (`yes` or `no`), or send it in a new message (`message`).

`code` - The code to eval.

## Example
```
bot.command({
    type: "command",
    name: "eval",
    code: `$eval[message;$message]`
})
```
