# OshiStories
Telegram bot to download your idol's latest media stories and posts

### Requirements
* [Python 3](https://www.python.org/)
* [Redis](https://redis.io)
* [Docker](https://docker.com)

### Settings before run
1. rename .env.example to .env
2. Add instagram username to OSHI_USERNAME with comma separated

### How To Create & Get BOT Token
[BotFather](https://www.siteguarding.com/en/how-to-get-telegram-bot-api-token)

### How To Get CHAT ID
1. Add bot as your friend & start chat
2. Open 
```
https://api.telegram.org/bot<YOUR_BOT_TOKEN>/getUpdates
```
![alt text](./screenshot-get-chat_id.png)

### Build Docker Images
```bash
$ docker build -t oshi-stories .
```

### Run Docker Container
```bash
$ docker run -it --rm --name oshi-stories-container -d oshi-stories
```