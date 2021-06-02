# $createDM
Creates a DM channel with a user.

## Usage
```
$createDM[userID;returnDMChannelID (yes/no)]
```

### Breakdown
`userID` - The user to create the DM channel with.

`returnDMChannelID` - 'yes' means the ID of the DM channel is returned (if creation is successful). 'no' means it isn't.

## Example
```js
bot.command({
    type: "command",
    name: "dm-id",
    code: `Your DM channel ID is $createDM[$authorID;yes].`
})
```
