# How to Connect R to Discord
To be able to delete messages from Discord, R needs specific credentials. Here I describe the working apprach to achive this. Caution: sending numerous requests to Discord causes it to blck the Bot.

1. Login into your account and create a channel

<p align="center">
<img src="https://github.com/Camilo-Mora/ConnectR_to_Discord/blob/main/Images/CreateChannel.png" width=50% >
</p>

Follow the instructions.

2. Unnecessary categories...right click on category (red arroad) and then on Delete category.

<p align="center">
<img src="https://github.com/Camilo-Mora/ConnectR_to_Discord/blob/main/Images/Clear.png" width=50% >
</p>

3. Get channel ID. Right click on #General, then on copy Channel ID

<p align="center">
<img src="https://github.com/Camilo-Mora/ConnectR_to_Discord/blob/main/Images/ChanelID.png" width=50% >
</p>

4. Create webhook. Needed for TV to send messages and for R to send delete messages.
Click on Edit Channel.
<p align="center">
<img src="https://github.com/Camilo-Mora/ConnectR_to_Discord/blob/main/Images/WEbHook.png" width=50% >
</p>

Then on Integrations and WEbhooks.
<p align="center">
<img src="https://github.com/Camilo-Mora/ConnectR_to_Discord/blob/main/Images/Integrations.png" width=50% >
</p>

Then on new webhook or exiting one. Copy the Webhook, which is used in TV and R.

<p align="center">
<img src="https://github.com/Camilo-Mora/ConnectR_to_Discord/blob/main/Images/WEbHook.png" width=50% >
</p>

5. Add a new Bot. This is basically the connectivity used by R to reach discord. from here we need a TOKEN, and install the bot in the channel.
   With the discord open, open this URL: https://discord.com/developers/applications

then click on existing or new one.

<p align="center">
<img src="https://github.com/Camilo-Mora/ConnectR_to_Discord/blob/main/Images/BOT.png" width=50% >
</p>

Click on BOT, then define the settings, like administrator. Then click on reset token, then copy it.
<p align="center">
<img src="https://github.com/Camilo-Mora/ConnectR_to_Discord/blob/main/Images/BotToken.png" width=50% >
</p>


Bot setteing, if you want to read messages, this information requires an intent that is privilage, so you need to specify that by ensuring the bot has the priviligy to read messages.

[here](https://discordjs.guide/popular-topics/intents.html#error-disallowed-intents)

<p align="center">
<img src="https://github.com/Camilo-Mora/ConnectR_to_Discord/blob/main/Images/Privilegies.png" width=50% >
</p>

6. Load the Bot in the channel. Got to OAUTHo2 and then to URL generator.. tick on Bot, and admisnistrator..at the bottom should appear a URL, copy and paste it in your browser, hit Enter
<p align="center">
<img src="https://github.com/Camilo-Mora/ConnectR_to_Discord/blob/main/Images/RegisterBot.png" width=50% >
</p>






Select the channel to which you want to add the BOT. Click Continue and then Autorize.
<p align="center">
<img src="https://github.com/Camilo-Mora/ConnectR_to_Discord/blob/main/Images/Auto.png" width=50% >
</p>

You are set. With the approach above you obtained Channel ID, Webhook for channel, and Token.

NOTE: in R, the Token need to be preceeded with the word "Bot TOKEN" like "Bot MTA3NjM2M...."
