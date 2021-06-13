# $isHoisted
Returns whether or not a role is displayed-seprately (hoisted). 

![image](https://user-images.githubusercontent.com/69215413/121823023-9a2d5e00-cc70-11eb-99b7-dfc3cec356a6.png)

> 'true' means the role is hoisted, 'false' means it isn't.

## Usage
```
$isHoisted[guildID;roleID]
```

### Breakdown
`guildID` - The server that the role belongs to.

`roleID` - The role to get the data for.

## Example
```js
bot.command({
    type: "command",
    name: "random-example",
    code: `$isHoisted[$guildID;837400697351045171]`
})
```
