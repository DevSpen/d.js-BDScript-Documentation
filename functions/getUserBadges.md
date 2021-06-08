# $getUserBadges
Displays all the badges of an user. 

## Usage 
`$getUserBadges[userID;separator]`

### Breakdown 
`userID` - ID of the user who's badges has to be displayed.

`separator` - Symbol or text the output has to be split with.

## Example
```
bot.command({
    type:"command"
    name:"badges"
    code:`
$getUserBadges // returns authors badges
//or
$getUserBadges[739591551155437654;,]
`
})
```
[WarningMsg] This function will display every badge except for nitro badges. All badges displayable is listed [here](https://discord.com/developers/docs/resources/user#user-object-user-flags)
