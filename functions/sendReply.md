# $sendReply
[Replies](https://support.discord.com/hc/en-us/articles/360057382374-Replies-FAQ) to the provided 'messageID'.

## Usage
```
$sendReply[messageID;message;(optional) returnMessageID (yes/no);(optional) disableMention (yes/no)]
```

### Breakdown
`messageID` - The message to reply to. Use `$messageID` for the author's message.

`message` - The message to send as the reply.

`returnMessageID` - Whether to return the bot's reply message ID in a new message or not. Default is `no`.

`disableMention` - If `no` the user will be mentioned when the bot replies. If `yes` the bot will not mention the user when it replies. Default is `no.`

## Example
```js
bot.command({
    type: "command",
    name: "sayhi",
    code: `$sendReply[$messageID;Hi!]`
})
```
