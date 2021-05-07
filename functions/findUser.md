# $findUser
Finds a user using username, ID, or mention.

## Usage
```$findUser[user;returnAuthorID (yes/no)]```

### Breakdown

`user` - The user `username`, `ID` or `mention` to find.

`returnAuthorID` - Whether to return the author ID if no user was found. Default is `yes`.


## Example
```
bot.command({
    type: "command",
    name: "find-user",
    code: `
    $findUser[$message;no] //Returns the user ID as the result.
    `
})
```
