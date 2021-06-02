# $cpu
Returns current CPU load of the machine in the last minute, as a percent.

## Usage
```
$cpu
```

## Example
```js
bot.command({
 type: "command",
 name: "cpu"
 code: `CPU Load: $cpu`
 })
````
