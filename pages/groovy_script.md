---
layout: page
title: QuPath Groovy script
---

Copy the following script into a text editor, and save it as `Telegram script ending.groovy`

```
// Telegram notifier - QuPath/Groovy section
// Groovy script to call Python script, which sends alert via Telegram.
// Edit Python script to change alert message.

def AlertInfo = ["python", "e:/QuPath/Utilities/Telegram/qupath_telegram_alert.py"]
def cmd = AlertInfo.execute()
cmd.waitForOrKill(1000)
println cmd.text
```

- Edit the line which points to where you saved the Python script, to point to its location on your computer.
<br>
When you want an alert sent, paste this code at the end of your QuPath script.
