# Introduction
d.js-BDScript is a cross between Bot Designer For Discord and discord.js. This language was developed for people who want to create easily create advanced bots. It has the flexibility of discord.js and the simplicity of BDScript functions. 

## Install
Here is how to install d.js-BDScript. Remember to use the shell for this.

```npm i d.js-bdscript```

## Setup
This is the "base" of your code per-say. 
```const bdjs = require("d.js-bdscript")
const bot = new bdjs({
    token: "token here", //bot token
    prefix: "prefix" //accepts an array of prefixes too 
})

bot.login()
bot.addEvent("onMessage")
bot.command({
    type: "command", //the command type
    name: "say", //command trigger
    code: "$message"
})
```
[Info Msg] Replace "token here" with your bot's token and "prefix" with your bot's prefix

## Updating
This makes sure the package is updated and ready to go. If your getting errors from `node (main file name)` or your bot is offline, try this then run `node (main file name)` again.
- First, run the text below in the shell.

```wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.37.2/install.sh | bash```

- Second, run the text below in the shell. Do this after running the first.

```export NVM_DIR="$HOME/.nvm" &&
[ -s "$NVM_DIR/nvm.sh" ] && . "$NVM_DIR/nvm.sh" &&
[ -s "$NVM_DIR/bash_completion" ] && . "$NVM_DIR/bash_completion" &&

nvm install --lts &&
nvm use --lts
```

## Getting Your Bot Online
To make your bot go "online" type `node (main file name)` into shell. For most, this would be `node index`. If you want to make it go offline do CTRL + C in the shell.
