# $checkContains
Checks if the message contains of the given word(s). The bot will return "true" if the text contains atleast one of the provided words. The bot will return "false" it doesn't.

## Usage
```$checkContains[text;word(s)]```

### Breakdown
`text` - The Text that you want to check if the Text contains of the given Word.

`word(s)` - The word or words to check, arguments separated by `;`.

## Example
```
bot.command({
 type: "command",
 name: "check-contains"
 code: `Does your message contain "dog"?: $checkContains[$message;dog]`
 })
````
