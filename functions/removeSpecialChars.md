# $removeSpecialChars
Removes special characters from the provided 'text'.

## Usage
```
$removeSpecialChars[text;removeNumbers (yes/no)]
```

### Breakdown
`text` - The text to remove special characters from.

`removeNumbers` - 'yes' means that numbers will be removed. 'no' means numbers will not be removed.

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `$removeSpecialChars[Hi! How are you? 123 #$#@;no]`
    // Returns "Hi How are you 123"
})
```
