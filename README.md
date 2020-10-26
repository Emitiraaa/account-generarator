# ![logo](https://i.imgur.com/aHRDloT.png)
## 🚩 Table of Contents
- [About](#-about)
- [How it works](#-works)
- [Examples](#-examples)

## ❓ About
This tool let your server's users to get accounts through a secure and advanced system.  
The accounts are saved in JSON files.  
The JSON file's name is the name of the service your users can generate accounts from.  
For example, if you have some netflix account you want to give, just create a netflix.json file or use the command /add netflix username:password.

## V3 Changelog
V3 is the biggest update this bot ever had.  
What's changed is EVERYTHING, the code has been completely rewrote.  
- JSON is used instead of TXT files, this makes everything easier and faster. 
- Create command has been removed, now you can just write add, and if the service do not exists, the bot will create it for you.  
- Cooldown and Prefix can be changed thorugh the command "change OPTION VALUE" example: "change prefix /". 
- Now you can check how many accounts are in a service.
- Stock command added to see all the stock.

## ⚙️ How it works
**Adding Accounts**  
You can add account to your servide through the command `/add` followed by the service and then the username and password in this syntax: username:password
  
**Receiving accounts**  
The user needs just to run the command `/gen` followed by the service's name and he will receive the account in DM.  
There is a 15 minutes cooldown by default, it can be changed in settings.json or through the command.
  
**Note**  
In the source code remember to replace "Channel ID" in the 
```js 
if (message.channel.id !== "Channel_ID") return
```
with the id of the channel you want the bot to work in.

## 🐾 Examples
/add netflix useraname1:password1 - This will add that account to the Netflix service  
/gen netflix - This will take the first account in the Netflix.json file and send it to the user 
/check Netflix - You will receive a message with the amount of accounts on that service.  
/stock - See the whole stock

