# $removeSpacing
Removes excess spacing from the provided text.


## Example
```
$removeSpacing[text]
```

### Breakdown
`text` - The text to apply the effect to.

## Example
```js
bot.command({
    type: "command", 
    name: "example", 
    code: `$removeSpacing[Hello     Everyone!]`
    // Returns 'Hello Everyone!'.
})
```
