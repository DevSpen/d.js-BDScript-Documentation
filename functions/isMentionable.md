# $isMentionable
Returns whether or not a role is mentionable by everyone.

![image](https://user-images.githubusercontent.com/69215413/121823186-8afae000-cc71-11eb-9f21-6b6e3af321e9.png)

> 'true' means the role is mentionable, 'false' means it isn't.

## Usage
```
$isMentionable[guildID;roleID]
```

### Breakdown
`guildID` - The server that the role belongs to.

`roleID` - The role to get the data for.

## Example
```js
bot.command({
    type: "command",
    name: "random-example",
    code: `$isMentionable[$guildID;837400697351045171]`
})
```
