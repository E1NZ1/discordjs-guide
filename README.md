# Discordjs-guide
Do you also Want to know discord.js. Watch this guide.
- Begginer Level
---
# Languages Used
- Node.js
- JavaScript

# Packages Used
- Discord.js v14

---
# Requirements
- Basic Knowledge of Js

---
# Getting Started
> OK so Before getting started I want to say what I am going to teach in this guide with you.
- How to Use Modals, Buttons, SelectMenus, Options, etc.
- How to make basic commands like ping, help.

# Handler
- Ok so you will need an nice handler if you want to code. So for the handler I will give you a nice handler. [So Click me]

# Creating Basic Commands
## How to create One?
### Here is an example of creating an command.
```js
module.exports = {
    name: "example", // the name of the slash Command
    description: "example command", // description to show below the command name,
    default_member_permissions: ["SendMessages", "BanMembers"], // the default_member_permissions.
    run: async (client, interaction) => {
        // Code
    }
}
```
- This is a sls command example.
  - Note: This is for our handler only.

# Replying to Slash Commands
So you will need to reply to an slash command to make an simple bot right?
```js
await interaction.reply(`Hi`)
```
Or
```js
await interaction.reply({ content: `Hi` })
```
# Creating Embeds
Ok so now let's start with Creating embeds
- Put this at the top of code
```js
const { EmbedBuilder } = require("discord.js")
```
- inside the code
```js
const embed = new EmbedBuilder()
.setTitle("Some Title")
.setDescription("some description")
.setFooter({ text: `Hi` })

await interaction.reply({ embeds: [embed] })
```
