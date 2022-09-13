## CEG-3120 Project 1

Jonathan Moseley

## Discord Bot documentation

1. Setup
   1. Dependencies needed: Python3, pip3, dotenv, discord.py
   
   2. How to get an API token: When a new bot is created you request an API token by using the 2FA code setup with discord. This must be copied as discord will not show it again
   
   3. Where to put API token in code: create a seperate file called .env where the API token will go in a DISCORD_TOKEN variable. 
   (This file ***must*** be put in the .gitignore file to disable git tracking and potental lekage of the sensitive API token)
   
2. Usage
   With your changes to the code in place, describe:
   1. What commands can you type in your discord server: Command to use is ```code%``` 
   
   2.  What response this will provde from your bot: The response will be parts of the RMS GNU/Linux copypasta
       
   Usage Screenshot:
   ![Discord_Screenshot](https://github.com/WSU-kduncan/ceg3120-Jmoseley512/blob/main/Discord-Bot/Bot.png)
   
3. Research
  To make this run in an 'always-on' state user can set this up as a system servivce with systemD via:
  
   ```systemctl start python bot_v9.py``` 
   
   and 
   
   ```systemctl enable python bot_v9.py``` 
   
  By setting this up as a system service and enabling it to run at boot the bot will always run when the server is running. This would work, as the server will need to do other things besides just running the single command to run the bot. As a system service a admin or user does not need to think about running the command to start the program even in the case of a restart as it will be configured to start at boot. 
