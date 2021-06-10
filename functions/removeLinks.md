# $removeLinks
Removes all links from the provided text.

## Usage
```
$removeLinks[text]
```

### Breakdown
`text` - The text to remove links from.

## Example
```js
bot.command({
    type: "command", 
    name: "example", 
    code: `$removeLinks[Hey everyone! https://google.com]`
    // Returns 'Hey everyone!'.
})
```
