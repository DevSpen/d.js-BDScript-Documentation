# $getUserBadges
Displays all the badges for a certain user.

## Usage 
`$getUserBadges[userID;separator]`

### Breakdown 
`userID` - The ID of the user who's badges are being displayed.

`separator` - The character(s) to split the different badge names with.

## Example
```js
bot.command({
    type: "command",
    name: "badges",
    code: `$getUserBadges // Returns authors badges.
// Or
$getUserBadges[739591551155437654;,] // Returns the provided user's badges.`
})
```
[WarningMsg] This function will display every badge except for Boosting/Nitro badges. All badges displayable are listed [here](https://discord.com/developers/docs/resources/user#user-object-user-flags).

