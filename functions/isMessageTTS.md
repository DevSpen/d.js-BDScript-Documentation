# $isMessageTTS
Returns whether or not the author's message was sent as text-to-speech (TTS).

> 'true' means the message is TTS, 'false' means it isn't.

## Usage
```
$isMessageTTS
```

## Example
```js
bot.command({
    type: "command",
    name: "example",
    code: `Was Your Message TTS? $isMessageTTS`
})
```
