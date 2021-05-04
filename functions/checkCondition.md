# $checkCondition
Checks whether given condition is false or true.

## Usage
```$checkCondition[condition]```

### Breakdown
`condition` - the condition to check.

## Example
```
bot.command({
    type: "command",
    name: "check-condition",
    code: `Is 3 greater than 2?: $checkCondition[3>2] //Returns true as the answer.
    `
})
```
