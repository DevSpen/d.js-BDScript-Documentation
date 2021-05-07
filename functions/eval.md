# $eval
Evals a d.js-bdscript code.

## Usage
```$eval[showOutput (message/boolean);code]```

### Breakdown

`showOutput` - Whether to return the output or send it in a new message or no.

`code` - The code to eval.


## Example
```
bot.command({
    type: "command",
    name: "$eval",
    code: `
    $eval[message;$ping] //Returns the bot's ping. You can eval a code from $message.
    `
})
```
