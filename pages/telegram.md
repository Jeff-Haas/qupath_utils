---
layout: page
title: Telegram Messenger alerts
tagline: Notifications when a script is done
description: 
---

This shows you how to set up Telegram Messenger to notify you when a QuPath script is done.  I have found that Telegram is much quicker to send messages than email, and once this is set up, the amount of code needed is very minimal.

There are a lot of steps here, but they go really quickly.

- [Python Installation](python_install.html)
- [Set up Telegram Messenger on your computer](telegram_setup.html)
- [Configure Python](python_install.html)
- [Test - Send a message](test_message.html)
- [Telegram smartphone app](telegram_app.html)
- [Python script](python_script.html)
- [QuPath Groovy script](groovy_script.html)


### Acknowledgments<br>
I've got a 3D printer and use a Raspberry Pi, running [Octoprint](https://octoprint.org/), to manage it.  One of the more useful plug-ins for Octoprint is a [Telegram alert module](https://github.com/fabianonline/OctoPrint-Telegram), which among many other features, sends you an alert when your print is done.  This is like QuPath running a long script, so I've adapted the concept.

I started with this post on Medium:
[Telegram bot with Python](https://medium.com/@robertbracco1/how-to-write-a-telegram-bot-to-send-messages-with-python-bcdf45d0a580).
However, since the post was written, there have been a few changes to the steps involved, and I've also added specific info for QuPath users.
