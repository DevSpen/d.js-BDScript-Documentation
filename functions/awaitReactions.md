# $awaitReactions
Awaits reactions on a certain message.

## Usage
```$awaitReactions[channelID;messageID;filter;time;emoji;max;code;error]```

### Breakdown
`channelID` - The channel ID where the message was sent in.

`messageID` - The message ID of the message the bot awaits reaction(s) for.

`filter` - Accepts user IDs. If multiple users are provided, separate them with commas (`,`). You can also use everyone for anyone's reaction to be accepted.

`time` - How long the bot will wait for the reactions to be added.

`emoji` - The emoji that the bot awaits the reaction(s) for.

`max` - The number of reactions to await (by different users) before running the `code`. If there aren't enough reactions added in the provided time, then the `error` message is returned.

`code` - The code to execute once all needed reactions are added.

`error` - The code to execute in case not enough reactions were added in the provided `time`.

## Example
```
bot.command({
    type: "command",
    name: "respects",
    code: `$awaitReactions[$channelID;$messageID;everyone;1m;🪦;3;$channelSendMessage[$channelID;3 People paid respects!;no];Not enough people paid respects.]
           $addMessageReactions[$channelID;$messageID;🪦]`
})
```
