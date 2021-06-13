# $isUserDMEnabled
Checks whether or not the bot can DM the user.
> 'true' means the bot can DM the user, 'false' means it can't.

## Usage
```
$isUserDMEnabled[(optional) userID]
```

### Breakdown
`userID` - The user to check. If this field is left empty, the bot checks the author's DM status.

## Example
```js
  bot.command({
    type: "command", 
    name: "hi", 
    code: `$onlyIf[$isUserDMEnabled==true;Please enable your DMs so I can send the message.]
    $sendDM[$authorID;Hi!;no]`
})
```
