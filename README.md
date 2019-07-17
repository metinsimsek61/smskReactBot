# Discord-RoleReact

A bot that automatically assigns roles based on message reactions.

![Demo of Bot using Regular Messages](https://i.imgur.com/AiukVfw.gif)

![Demo of Bot Using Embeds](https://i.imgur.com/ynmL2qb.gif)

## Features

- Customizable messages, reactions, commands, and roles

- Auto-removes role when user removes a reaction

- Option to use an embed to have all options in one message

- Error handling to let you know if something is wrong

## Installation

Clone this repository to your local machine.

Run the `npm install` command to install discord.js

Open `roleReact.js` with a text editor and modify the following lines: 

```JavaScript
const yourID = "158063324699951104"; //Instructions on how to get this: https://redd.it/40zgse
const setupCMD = "!createrolemessage";
const initialMessage = `**React to the messages below to receive the associated role. If you would like to remove the role, simply remove your reaction!**`;
const embedMessage = `
React to the emoji that matches the role you wish to receive.

If you would like to remove the role, simply remove your reaction!
`;
const embedFooter = "Role Reactions"; // Must set this if "embed" is set to true
const roles = ["Hacker", "Artist", "Public Relations", "Intern"];
const reactions = ["💻", "🖌", "😃", "🆕"]; // For custom emojis, provide the name of the emoji
const embed = false; // Set to "true" if you want all roles to be in a single embed
const embedColor = "#dd2423"; // Set the embed color if the "embed" variable is set to true
const embedThumbnail = true; // Set to "true" if you want to set a thumbnail in the embed
const embedThumbnailLink = "https://i.imgur.com/P8PD7DD.png"; // The link for the embed thumbnail
const botToken = "";
/**
 * You'll have to set this up yourself! Read more below:
 * 
 * https://github.com/reactiflux/discord-irc/wiki/Creating-a-discord-bot-&-getting-a-token
 */
```

Mandatory:

- Fill in the `yourID` variable. You can get `yourID` in any Discord channel by typing `\@YOUR NAME`. For me, it would be `\@Night`.

- Change roles the to ones that are in your server.

- Replace the reaction emojis with the ones of your choosing. 
**Note:** to get the value for the reaction, type `\:my_reaction` with the backslash and press enter. If done correctly, a smaller emoji should appear. Copy the small emoji into the reactions array.
 For custom emojis, simply provide the name of the custom emoji that you wish to use.

- Set `embed` to true or false if you wish to use a single embed for all reaction roles. After that, set the text for the embed footer via the `embedFooter` variable

- Set up the bot and get a token. The [Github Wiki Page](https://github.com/reactiflux/discord-irc/wiki/Creating-a-discord-bot-&-getting-a-token) explains how to set up bots and get tokens. An image of the permissions the bot needs can be [found here](https://i.imgur.com/PFDm3pH.png). **Make sure the bot has a role/the permissions that allows it to modify other user's roles.**

Optional:

- Modify the `setupCMD` variable to display a custom setup message

- Modify `initialMessage` variable to display a custom initial message

- Modify the `embedMessage` variable to display a custom message for the embed

- Modify the `embedColor` variable to display a custom embed color

**After you have installed discord.js and made the modifications above, run the `npm start` command to start the bot!**

## Support

I hope you find this bot useful. If you need help or find any bugs, use the appropriate forums in this repository to contact me.
