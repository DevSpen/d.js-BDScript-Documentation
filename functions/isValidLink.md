# $isValidLink
Returns whether or not the provided link is valid.
> 'true' means the link is valid, 'false' means it isn't.

## Usage
```
$isValidLink[link]
```

### Breakdown
`link` - The link to check.

## Example
```js
  bot.command({
    type: "command", 
    name: "hi", 
    code: `$onlyIf[$argCount[$message]>=1;Please provide text!]
    Is $message a valid link?: $isValidLink[$message]`
})
```
