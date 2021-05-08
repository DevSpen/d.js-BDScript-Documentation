# $divide
Divides the provided numbers.

## Usage
```$divide[numbers]```

### Breakdown
`numbers` - Number(s) to divide, separated by `;`.


## Example
```
bot.command({
    type: "command",
    name: "divide",
    code: `$divide[$message[1];$message[2]]
    $onlyIf[$argCount==2;Please use this format: !divide (number1) (number2)]`
})
```
