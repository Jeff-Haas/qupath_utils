---
layout: page
title: Telegram Messenger alerts
tagline: Notifications when a script is done
description: Overview of construction of a website with GitHub Pages
---

I've got a 3D printer and use a Raspberry Pi, running Octoprint, to manage it.  One of the more useful plug-ins for Octoprint is a Telegram alert module, which sends you an alert when your print is done.  This is like QuPath running a long script, so I've adapted the concept.

There are a lot of steps here, but they go really quickly.

- Install Python:
Go to [Python] (https://www.python.org/)
Click "Downloads" and pick the version for your machine.

- Add Python to your computer's shell path.  This lets you run Python from any folder on your computer, so QuPath can call it from where it is installed.

For Windows, select the box at the bottom of the install dialog, then click "Install Now".
[screenshot]

For Macintosh, I need advice from a Mac user.



- Install Telegram on your computer and set up an account.
[Telegram Messenger] (https://telegram.org/)

- Configure Telegram:
Click this link to access the Telegram "BotFather", which is their utility to configure automatic responses, or "bots":
[BotFather] (https://telegram.me/BotFather)
It will open Telegram on your computer, to the BotFather account.

- Send the message "/newbot" (no quotes) to BotFather by clicking Start at the bottom of the window, and follow the instructions that come back.  You will answer two questions (naming your bot) and then it will display a bunch of text.  I suggest you copy the block of text into a document and save it, it has your token to access the Telegram API.

You have set up your Telegram account and added an auto-responding "bot" to it.


Now it's time to set up Python on the computer, so it can talk to Telegram.

- Open a Command Prompt (this is not the Python command prompt.) For Windows 10, click the magnifying glass on the taskbar, type "Command Prompt" and press enter.
[screenshot]


Then copy and paste this line into the Command Prompt, and hit enter:
pip install telegram-send
This will tell Python to install the Telegram sender software.

Then copy and paste this line into the Command Prompt, and hit enter:
telegram-send --configure
This tells Python to configure the Telegram sender.


In the Command Prompt window, telegram-send will ask for the token you got from the BotFather.  Copy the token and paste it into the Command Prompt window.

Then telegram-send will give you a password that you need to message to your new bot in the Telegram app.


Telegram will reply in the Command Prompt window with a URL.  Copy the URL and paste it into a browser address bar.  It will open your Telegram app to the right window to talk to the new bot.  In the Telegram app, click the Start button to talk to the bot and send it the password from the Command Prompt window.

You should see a reply in the Command Prompt window that telegram-send is ready for use.  The Telegram app should also show that it's ready for use.

You're nearly done.  Now to test it!

- Send a message from Python to Telegram

Open a Python command prompt window - this is different than the standard Windows Command Prompt!
[screenshot of Python window]

Paste the following test message into the Python window:

import telegram_send
telegram_send.send(messages=["Wow that was easy!"])

When you press Enter, you should see "Wow that was easy!" pop up as a message in the Telegram app.

Python is now configured to send messages to Telegram.

- Install the app on your smartphone and log into it.  Any message sent to your new bot will show up both in the app on your computer and on your phone.  You don't need to have the version on your computer running, you can just have the app on your phone.

- Save qupath_telegram_alert.py to a folder on your hard drive.  You can edit the message on line 6 if you need to.

- Edit line 5 of Telegram script ending.groovy so the path points to the location of qupath_telegram_alert.py on your computer.

- When you want to be notified that a QuPath script is done, paste Telegram script ending.groovy at the end of the script.


Acknowledgment
I started with this post on Medium:
[How to write a Telegram bot] (https://medium.com/@robertbracco1/how-to-write-a-telegram-bot-to-send-messages-with-python-bcdf45d0a580)
However, since the post was written, there have been a few changes to the steps involved, and I've also added specific info for QuPath users.
