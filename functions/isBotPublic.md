# $isBotPublic
Returns whether or not the bot is public.
> 'true' means the bot is public, 'false' means it isn't.

![image](https://user-images.githubusercontent.com/69215413/122114017-cf60ba00-cdf0-11eb-91f7-389895b252b4.png)

*Preview of the Setting*

## Usage
```
$isBotPublic
```

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `Am I Public? $isBotPublic`
})
```
