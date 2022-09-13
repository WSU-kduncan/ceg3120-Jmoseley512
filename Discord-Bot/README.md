## Jonathan Moseley
## CEG-3120
## Project 1

## Discord Bot documentation

1. Setup
   Dependencies needed: Python, pip, dotenv, discord.py
   How to get an API token: When a new bot is created you request an API token by using the 2FA code setup with discord. 
   Where to put API token in code: create a seperate file called .env where the API token will go in a DISCORD_TOKEN variable. (This file must be put in a .gitignore file to disable tracking)
2. Usage
   With your changes to the code in place, describe:
       1. What commands can you type in your discord server: In the server I can type code% 
       2. What response this will provde from your bot: The response will be parts of the RMS GNU/Linux copypasta
   Screenshots:
   ![Discord_Screenshot](https://github.com/WSU-kduncan/ceg3120-Jmoseley512/blob/main/Discord-Bot/Bot.png)
3. Research
   A possible solution to make this bot run without needing to run the command would be to either use GNU Screen and have this bot running in the background with it. 
   Additionally a user can set this up as a system servivce with systemD via ```systemctl start python bot_v9.py``` and ```systemctl enable python bot_v9.py``` so that the program will automatically start at boot without the user needing to manually start the program. 
