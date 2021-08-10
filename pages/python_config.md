---
layout: page
title: Configuring Python
---

Now it's time to set up Python on the computer, so it can talk to Telegram.

- Open a Command Prompt (the system command prompt, not the Python command prompt.) For Windows 10, click the magnifying glass on the taskbar, type "Command Prompt" and press Enter to get this window:

![image](https://user-images.githubusercontent.com/27331078/128942296-b9db3ca2-1e0f-417b-97b9-201880627223.png)


Then copy and paste this line into the Command Prompt, and hit enter:

`pip install telegram-send`

This will tell Python to install the Telegram sender software.

When that's done, copy and paste this line into the Command Prompt, and hit enter:

`telegram-send --configure`

This tells Python to configure the Telegram sender.


In the Command Prompt window, telegram-send will ask for the token you got from the BotFather.  Copy the token and paste it into the Command Prompt window.

telegram-send will give you a password to send to your new bot in the Telegram app.


In the Command Prompt window, Telegram will give you a URL.  Copy the URL and paste it into a browser address bar.  It opens your Telegram app to the right window to talk to the new bot.  Click the Start button to talk to the bot, and send it the password from the Command Prompt window.

- You should see a reply in the Command Prompt window that telegram-send is ready for use.
- The Telegram app should also show a message from the bot that it's ready for use.

You're nearly done.  Now to test it!

### Next:
- [Test - Send a message](test_message.html)

##### Back to top:
- [Telegram Messenger](telegram.html)
