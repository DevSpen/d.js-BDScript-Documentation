# $clearEmbed
Clears the current built embed.

## Usage
```$clearEmbed```

## Example
```
bot.command({
    type: "command",
    name: "check-condition",
    code: `$clearEmbed
    $description[nya] //Embeds will not be delivered as response.
    `
})
```
