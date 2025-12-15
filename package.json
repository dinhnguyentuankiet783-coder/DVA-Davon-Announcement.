const { Client, GatewayIntentBits } = require("discord.js");

const client = new Client({
  intents: [
    GatewayIntentBits.Guilds,
    GatewayIntentBits.GuildMessages,
    GatewayIntentBits.MessageContent
  ]
});

client.once("ready", () => {
  console.log("Bot online");
});

client.on("messageCreate", msg => {
  if (msg.content === "ping") {
    msg.reply("pong");
  }
});

client.login(process.env.TOKEN);
