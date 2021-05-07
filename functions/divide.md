# $divide
Divides numbers

## Usage
```$divide[value1;value2]```


### Breakdown

`value1 / value2` - The numbers to divide.


## Example
```
bot.command({
    type: "command",
    name: "divide",
    code: `
    30 / 5 = $divide[30;5]
    `
})`
