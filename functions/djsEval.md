# $djsEval
Evals JavaScript code.

## Usage
```$djsEval[showOutput (yes/no);code]```

### Breakdown
`showOutput` - Whether to return the evaled code.

`code` - The code to eval.

## Example
```
bot.command({
    type: "command",
    name: "djs-eval",
    code: `$djsEval[yes;$message]`
})
```
