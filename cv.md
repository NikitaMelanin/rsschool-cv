# 1) Name
Nikita Melanin
# 2) Contacts
#### [VK](https://vk.com/preter_human)
#### Mail: cool.melanin@list.ru
# 3) About me
On real time, I'm a intern-beginner developer. I am a perfectionist, If I start doing something, I’m only gonna finish it when it’s perfect. I want to be a full-stack developer in the future. But the real time, my goal is to learn as much as posiible informations about programming/develop, also I’m interested in learning different languages - trying something new, standing in one place is not my.
# 4) Skills
At the university I studied C#, had experience in Unity, before I studied Python with pyp Django, but not for long, I developed bot's for Discord on JavaScript with Node.js
# 5) Example code
```javascript 
const Discord = require ('discord.js'); // framework discord.js
const client = new Discord.Client(); // client announcement
const comms = require ("./comms.js"); //add comnands
const fs = require ('fs'); // node.js module
const yt = require('ytdl-core');//player
const searchYoutube = require('youtube-api-v3-search');//search
const config = require ('./cfg.json'); // parm cfg client

let token = config.token;
let prefix = config.prefix;
let youtubeapi = config.youtube_api_key;
var queue = {};
    client.on('message', (message) => { // reaction on message
    if (message.author.username != client.user.username && message.author.discriminator != client.user.discriminator) {
      var comm = message.content.toLowerCase().trim() + " ";
      var comm_name = comm.slice(0, comm.indexOf(" "));
      var messArr = comm.split(" ");
      for (comm_count in comms.comms) {
        var comm2 = prefix + comms.comms[comm_count].name;
        if (comm2 == comm_name) {
          comms.comms[comm_count].out(client, message, messArr);
        }
      }
      if (!message.content.startsWith(config.prefix)) return;
    if (commands.hasOwnProperty(message.content.toLowerCase().slice(config.prefix.length).split(' ')[0])) commands[message.content.toLowerCase().slice(config.prefix.length).split(' ')[0]](message);
    }
  });
```
# 6) Expirience
I was at the university dev.team where we did a the Unity [game](https://drive.google.com/drive/folders/1VBdITsPAeUBK4-mQnWFpbi6iomVQAV3V)
# 7) Education
I'm study at the Urfu. 
# 8) English
My English is about B1-B2 lvl, as the English teacher told me )
