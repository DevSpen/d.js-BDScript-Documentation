# $getTextSplitLength
Returns the number of splits in `$textSplit`.

[WarningMsg] This function can not be used, if `$textSplit` isn't present in the code.

## Usage
```
$getTextSplitLength
```

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `$textSplit[hi | hello | hey;|]
    $getTextSplitLength`
    // Returns 3
})
