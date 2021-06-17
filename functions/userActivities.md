# $userActivities
Returns a user's status activities.

## Usage
```
$userActivities[userID;returnData;(optional) separator]
```

### Breakdown
`userID` - The user to get the status activities from.

`returnData` - The data to return, properties must be used inside `$data[]`. [(see activities properties)](https://djs-bdscript.gitbook.io/docs/properties/activity-properties)

`separator` - The separator between each data-piece (if needed). Default is `\n` (new line).

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `**$userTag[$mentioned[1;yes]]'s Status Details**
$userActivities[$mentioned[1;yes];
Name: $data[name]
Details: $data[details]
State: $data[state]
Type: $data[type]]`
})
```
