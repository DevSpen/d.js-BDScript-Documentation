# Activity Properties
A list of all activity properties, for functions like [$userActivities](https://djs-bdscript.gitbook.io/docs/useractivities).
  
- `createdTimestamp` - The time that this activity started (in milliseconds).
- `details` - The details of this activity.
- `emojiID` - The ID of the emoji, in this user's status.
- `emojiName` - The name of the emoji, in this user's status.
- `emojiURL` - The image URL of the emoji in this user's status.
- `emoji` - The stringified version of the emoji in this user's status.
- `name` - This activity name.
- `sessionID` - The session ID of this activity.
- `state`  The state of this activity.
- `type` - The activity type [(see activity types [sub-property])](https://djs-bdscript.gitbook.io/docs/properties/activity-properties#activity-types).

[InfoMsg] Properties and sub-properties run on a 'if any' basis. Meaning, if the user doesn't have the inputted property active: nothing, 'none', or 'null' can be returned.

## Sub-Properties

### Activity Types
A list of all activity types.
- `COMPETING`
- `LISTENING`
- `PLAYING`
- `STREAMING`
- `WATCHING`
