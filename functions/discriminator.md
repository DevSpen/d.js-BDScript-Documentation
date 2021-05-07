# $discriminator
Returns user's discriminator.

## Usage
```$discriminator[user ID (optional)]```

### Breakdown
`user ID` - The user to get the discriminator from. If no userID is provided, the bot will return the author's discriminator.

## Example
```
bot.command({
    type: "command",
    name: "me",
    code: `$username#$discriminator `
})
```
