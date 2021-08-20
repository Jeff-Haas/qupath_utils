---
layout: page
title: Send a test message
---

Open a Python command prompt window - this is different than the standard Windows Command Prompt!
- On Windows 10, open the Start menu and type "python" to find Python. <br>

![image](https://user-images.githubusercontent.com/27331078/128942559-518b9c17-d23d-4ab0-9880-424da601d461.png)

Paste the following test messages into the Python window:

`import telegram_send`
<br>
and press Enter.

`telegram_send.send(messages=["Wow, that was easy!"])`

Press Enter again and you should see "Wow that was easy!" pop up as a message in the Telegram app.

This shows that Python is now configured to send messages to Telegram.

### Next:
- [Python script](python_script.html)

##### Back to top:
- [Telegram Messenger](telegram.html)
