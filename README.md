```js
const { Client, GatewayIntentBits } = require('discord.js');
const client = new Client({ intents: [GatewayIntentBits.Guilds] });
const User = require('pokita.js')
require('dotenv').config();

client.on('ready', () => {
  console.log(`Profile Ready!`);
});

client.on('messageCreate', message => {

 if(message.content === "About Me"){
 return message.channel.send("
 Im Pokita
 I Like JS and Discord.js
 My Webpage: https://pokita.site/
 Founder of Cyclone Bot
 I like the vanilla ice cream so hard...
 ")}

client.login(process.env.pokita_token);
});
```
