# ttvLogs/logs-next

This bot is used to synchronize messages from the twitch chat with the database for further use on the site.

## Getting started

- install dependencies
- start bot


```
yarn
yarn start
```
or
```
pm2 start bot.js --cron "0 5 */7 * *" && pm2 monit
```

## Configuration

- create your .env file in root

```toml
#twitch bot
NICKNAME = "twith bot nickname"
TOKEN = "oauth:token"

#database
SERVERNAME = "server ip"
USERNAME = "user"
PASSWORD = "password"
DATABASE = "database name"

#bot options
PREFIX = "`"
ADMIN = "your nickname on twitch"
MAIN = "logs"
DEFAULTCHANNEL="default channel to connect"

#twitch api
BEARER = "Bearer token"
CLIENTID = "client id of your bot"
```
