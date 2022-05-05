```js
const Discord = require('Discord.js')
const intents = new Discord.Intents();
const client = new Discord.Client({ intents: 13839 });
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
