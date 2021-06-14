# $userReacted
Checks whether or not the provided user has reacted with the 'emoji' on a message.
> 'true' means the user did react with the 'emoji' on the provided message, otherwise 'false' is returned.

## Usage
```
$userReacted[channelID;messageID;userID;emoji]
```

### Breakdown
`channelID` - The channel that the message was sent in.

`messageID` - The message to get the reactions from.

`userID` - The user to get the reactions for.

`emoji` - The emoji to get the data from. Can be a unicode emoji or emoji ID.
