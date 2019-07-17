# Discord-RoleReact

A bot that automatically assigns roles based on message reactions.

![Demo of Bot using Regular Messages](https://i.imgur.com/AiukVfw.gif)

![Demo of Bot Using Embeds](https://i.imgur.com/ynmL2qb.gif)

## Features

- Customizable messages, reactions, command, and roles

- Auto-removes role when user removes a reaction

- Option to use an embed to have all options in one message

- Error handling to let you know if something is wrong

## Installation

Clone this repository to your local machine.

Run the `npm install` command to install discord.js

Open `config.js` with a text editor and modify the different properties to your liking. Most options are fairly straightforward, however, there is commenting where appropriate.


## Configuration
Mandatory:

- Fill in the `yourID` property with your User iD. You can get your User iD in any Discord channel by typing `\@YOUR NAME` or enabling "Developer Mode" in the Appearance section of your Discord settings. For example, you would do `\@anthony` to get [acollierr17](https://github.com/acollierr17)'s Discord User ID.

- Change roles the to ones that are in your server.

- Replace the reaction emojis with the ones of your choosing. 
**Note:** to get the value for the reaction, type `\:my_reaction:` with the backslash and press enter. If done correctly, a smaller emoji should appear. Copy the small emoji into the reactions array.
 For custom emojis, simply provide the name of the custom emoji that you wish to use.

- Set the `embed` property to true or false if you wish to use a single embed for all reaction roles. After that, set the text for the embed footer via the `embedFooter` property

- Set up the bot and get a token. The [Github Wiki Page](https://github.com/reactiflux/discord-irc/wiki/Creating-a-discord-bot-&-getting-a-token) explains how to set up bots and get tokens. An image of the permissions the bot needs can be [found here](https://i.imgur.com/PFDm3pH.png). **Make sure the bot has a role with the permissions that allows it to modify another user's roles.**

Optional:

- Modify the `setupCMD` property to display a custom setup message

- Modify `initialMessage` property to display a custom initial message

- Modify the `embedMessage` property to display a custom message for the embed

- Modify the `embedColor` property to display a custom embed color

- Modify the `setupCMD` property to a custom command to be used

- Modify the `deleteSetupCMD` property to delete the `setupCMD` message when it's ran

**After you have installed discord.js and made the modifications above, run the `npm start` command to start the bot!**

## Support

We hope you find this bot useful. If you need help or find any bugs, use the appropriate forums in this repository to contact us.
