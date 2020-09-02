# Rotating status plugin for modmailbot #
This is a plugin designed by [Eight8-7020](https://github.com/Eight8-7020) also known as Eight8#7020 on discord. If you need support on this, please ping me in #other-chatter in the main [support server](https://discord.gg/vRuhG9R).  

### Setup ###
Download and add the status folder into your ./src directory.  
Find the ```statuscfg.json``` file located in ./src/status/.  
Open it using a text editor like notepad, notepad++, vim, cat or nano.  
Edit the following values:  

## Adding the plugin to your config.ini file ##
In order to add the plugin to your config.ini, create a new line and add this:  
```plugins = ./src/status/status.js``` or if you have multiple plugins:  
```plugins[] = ./src/status/status.js```

## Status ##
You should currently see a line like ```"status":["STATUS1","STATUS2"];```  
Note that due to the status being a random pick, you can add more options by adding a comma after the last ```"STATUS"``` Like as follows: ```status:["STATUS1","STATUS2","STATUS3"]``` and so on. remember to wrap any statuses with ```""```  

## Time ##
This value should be set to the time (in miliseconds) that a status is rotated. please note anything under 15000 miliseconds will make your bot unusable.  
For example, if I wanted the bot to change its status every 115000 miliseconds, I would set it to ```"time":"11500"```.  

In order for changes to take affect, restart your bot.  
