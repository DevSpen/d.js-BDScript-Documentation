# $deleteGlobalUserData
Deletes all the variable values for given user.

## Usage
```
$deleteGlobalUserData[userID]
```

### Breakdown
`userID` - The user to delete the data from.

## Example
```js
bot.command({
 type: "command",
 name: "resetmydata"
 code: `$deleteGlobalUserData[$authorID]
 I have reset all your data!`
 })
 ```
