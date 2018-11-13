# Discord-RoleReact

A bot that automatically assigns roles based on message reactions.

![Demo of Bot](https://i.imgur.com/5vxxCDw.gif)

## Features

- Customizable messages, reactions, commands, and roles

- Auto-removes role when user removes a reaction

## Installation

Clone this repository to your local machine.

Uninstall any previous versions of discord.js module with `npm uninstall discord.js`. 

Install the latest version of discord.js module and then run `npm install discord.js --save`.

Open `roleReact.js` with a text editor and modify the following lines: 

```JavaScript
//Settings!
const yourID = ""; //Instructions on how to get this: https://redd.it/40zgse
const setupCMD = "!createrolemessage"
let initialMessage = `**React to the messages below to receive the associated role. If you would like to remove the role, simply remove your reaction!**`;
const roles = ["Hacker", "Artist", "Public Relations", "Intern"];
const reactions = ["💻", "🖌", "😃", "🆕"];
const botToken = ""; /*You'll have to set this yourself; read more
                     here https://github.com/reactiflux/discord-irc/wiki/Creating-a-discord-bot-&-getting-a-token*/
```

Mandatory:

- Fill in the yourID variable. You can get "yourID" in any discord channel by typing "\\@YOUR_NAME". For me, it would be \\@Night.

- Change roles the to ones that are in your server.

- Replace the reaction emojis with the ones of your choosing. 
**Note:** to get the value for the reaction, type `\:my_reaction` with the backslash and press enter. If done correctly, a smaller emoji should appear. Copy the small emoji into the reactions array.
For custom emojis, follow the previous step and copy the string of numbers only (i.e. ignore text and angled brackets). Paste the string of numbers into the reactions array as you would with regular emojis.

- Set up the bot and get a token. The [Github Wiki Page](https://github.com/reactiflux/discord-irc/wiki/Creating-a-discord-bot-&-getting-a-token) explains how to set up bots and get tokens. An image of the permissions the bot needs can be [found here](https://i.imgur.com/PFDm3pH.png). **Make sure the bot has a role that allows it to modify other user's roles.**

Optional:

- Modify the setupCMD to display a custom setup message.

- Modify initialMessage to display a custom initial message.


## Support

I hope you find this bot useful. If you need help or find any bugs, use the appropriate forums in this repository to contact me.
