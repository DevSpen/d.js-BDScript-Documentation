# Command Handler
## What Is "Command Handler"?
Command Handler can be used for organizing your bot's commands. Although recommended, its 100% optional.  

## Setup
In order to use the command handler, you must add the following code to your main file.
```js
bot.manager.load("./commands/")
// You should put this below 'onMessage' event.
```


### Main File Example
*(with command handler)*
```js
const bdjs = require("d.js-bdscript")
const bot = new bdjs({
    token: "token here",
    prefix: "prefix"
})

bot.login()
bot.addEvent("onMessage")
bot.manager.load("./commands/")
```

## Using Command Handler
1: Create a folder called "commands".

![image](https://user-images.githubusercontent.com/69215413/121552384-6cc98180-c9de-11eb-9bd4-6e94ff30884b.png)

2: Make a subfolder. (optional)

![image](https://user-images.githubusercontent.com/69215413/121552488-82d74200-c9de-11eb-9761-e53053108c4f.png)


3: Create the command using the base code below.
```js
module.exports = {
    type: "Type",
    name: "Name", 
    code: `Code`
}
```

### Example Code Using Command Handler
```js
module.exports = {
    type: "command",
    name: "ping", 
    code: `Pong! $ping ms`
}
```

![image](https://user-images.githubusercontent.com/69215413/121552642-9f737a00-c9de-11eb-806c-0692782cbdcc.png)

### Multiple Commands In One File
With command handler, you can create multiple commands inside one file. Example below:

[InfoMsg] This is only supported in version 5.0.0 and above.

```js
module.exports = [{
  type: "command",
  name: "hi",
  code: `Hello $username`
}, {
  name: "ping",
  code: `Pong! $ping ms`
}, {
  type: "joinCommand",
  channel: "39459438494840494",
  code: `<@$authorID> just joined the server!` 
}] // End the code with this.
```

<InfoMsg> This example uses [DanBot](https://danbot.host), but most other services support this feature!


