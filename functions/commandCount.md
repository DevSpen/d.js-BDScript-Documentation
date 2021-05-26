# $commandCount
Returns total command count or amount of certain type(s) of commands.

## Usages
### Usage #1
```js
$commandCount
// Returns the total command count.
```

### Usage #2
```js
$commandCount[types]
// Replace 'types' with a real command type.
// If you want to include multiple types, you can by separating them with ;

```
> [Click-me to view a list of all command types.](https://djsbdscript.gitbook.io/docs/command-types#types)

## Example
```js
bot.command({
    type: "command", 
    name: "command-count",
    code: `I have $commandCount commands!`
})
