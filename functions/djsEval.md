# $djsEval
Evals a javascript code.

## Usage
```$djsEval[showOutput (yes/no);code]```


### Breakdown

`showOutput` - Whether to return the evaled code. Default is `no`.

`code` - The code to eval.


## Example
```
bot.command({
    type: "command",
    name: "eval",
    code: `
    $djsEval[yes;let nya = 'nya'
    nya]
    `
})`
```


To eval the code from message,
```
bot.command({
    type: "command",
    name: "eval",
    cdoe: `
    $djsEval[yes;$message]
    `
})
