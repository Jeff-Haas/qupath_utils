---
layout: page
title: Telegram Messenger
tagline: Easy, fast alerts
description: 
---

This shows you how to set up Telegram Messenger to alert you when a QuPath script is done.  I have found that Telegram is much quicker to send messages than email, and once this is set up, the amount of code needed is very minimal.

### Summary
Set up an account with Telegram Messenger, and install Python on your computer.  Add a small script to the end of your QuPath script, which calls a small Python script.  The Python script sends a text message to the Telegram app on your smartphone.
<br>
<br>
Once this is set up, the only thing you need to do is paste a few lines into the end of a QuPath script.
<br>

### Setting up
There are a lot of steps here, but they go really quickly.

- [Python Installation](python_install.html)
- [Set up Telegram Messenger on your computer](telegram_setup.html)
- [Configure Python](python_install.html)
- [Test - Send a message](test_message.html)
- [Telegram smartphone app](telegram_app.html)
- [Python script](python_script.html)
- [QuPath Groovy script](groovy_script.html)


### Acknowledgments<br>
I've got a 3D printer and use a Raspberry Pi, running [Octoprint](https://octoprint.org/), to manage it.  One of the more useful plug-ins for Octoprint is a [Telegram alert module](https://github.com/fabianonline/OctoPrint-Telegram), which among many other features, sends you an alert when your print is done.  This workflow is like QuPath running a long script, so I've adapted the concept.

I started with this post on Medium:
[Telegram bot with Python](https://medium.com/@robertbracco1/how-to-write-a-telegram-bot-to-send-messages-with-python-bcdf45d0a580).
However, since the post was written, there have been a few changes to the steps involved, and I've also added specific info for QuPath users.
