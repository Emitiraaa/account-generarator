# ![logo](https://i.imgur.com/aHRDloT.png)
## 🚩 Table of Contents
- [About](#-about)
- [How it works](#-works)
- [Examples](#-examples)
- [Modules](#-modules)


## ❓ About
This tool let your server's users to get accounts through a secure and advanced system.  
The accounts are saved in txt files, so you do not have to deal with databases.  
You can create a service, and generate accounts for that service.  

## ⚙️ How it works
**Service creation**   
You have to create the services you provide account for. (netflix, etc..), use the command `/create`, this will create a txt file
with the name of the service you choosed, you can also create it manually.  
  
**Adding Accounts**  
After you created a service, you have to add accounts to it, you just have to use the command `/add` followed by username and password
in the next syntax username:password, and then the service's name  
  
**Receiving accounts**  
The user needs just to run the command `/gen` followed by the service's name and he will receive the account in DM.  
There is a 15 minutes cooldown that you can edit in the source code  
  
**Restocking accounts**  
After you filled the txt with all the accounts you want, you can use the command `/restock` followed by the service name to alert the users that the service has been restocked  
  
**Note**  
In the source code remember to replace "Channel ID" in the 
```js 
if (message.channel.id === "Channel_ID")
```
with the id of the channel you want the bot to work in.

## 🐾 Examples
/create Netflix - This will create a txt file with the name "Netflix"  
/add username1@gmail.com:password1 Netflix - This will add that account to the Netflix service  
/gen Netflix - This will take the first account in the Netflix.txt file and send it to the user  
/restock Netflix - The bot will send an @everyone message saying that Netflix' service has been restocked.  

## 📦 Modules

### discord.js
powerful node.js module that allows you to interact with the Discord API

### Async
utility module which provides straight-forward, powerful functions for working with asynchronous JavaScript

### Express
Fast, unopinionated, minimalist web framework for Node.js

###  Firstline
npm async module for NodeJS, that reads and returns the first line of any file.

### Line-reader
line-by-line file/stream reader with support for user-defined line separators.
