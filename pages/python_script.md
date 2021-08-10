---
layout: page
title: Python script
---

Copy the following Python script into a text editor, and save it as 
`qupath_telegram_alert.py`

- I suggest you set up a folder just for QuPath scripts.

```
# Telegram notifier - Python section
# Sends alert message to your Telegram account.
# Called from inside QuPath by Groovy script.

import telegram_send
telegram_send.send(messages=["QuPath workstation 1 - Task complete"])
print("Alert sent")
```
- To customize the message sent to Telegram, edit the telegram_send.send line.
- The "Alert sent" line will be shown in the QuPath script window.

### Next:
- [QuPath Groovy script](groovy_script.html)
