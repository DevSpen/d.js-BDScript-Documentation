# $serverBoostingSince
Returns how long a user has been boosting in milliseconds.

## Usage
```
$serverBoostingSince[guildID;userID]
```

### Breakdown
`guildID` - The server to get the data from.

`userID` - The user to get the data for.

> You can also use `$serverBoostingSince` without any fields, which will return how-long the author has been boosting in the current server.

## Example
```js
bot.command({
    type: "command", 
    name: "boost-time", 
    code: `$onlyIf[$isBoosting==true;You are not boosting!]
    You have been boosting since $formatDate[$serverBoostingSince;MMMM Do YYYY, h:mm:ss a]!`
})
```
