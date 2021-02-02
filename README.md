# Node-MongoDB Example (with Docker)

> Simple example of a dockerized Node/Mongo app

## Quick Start

```bash
# Run in Docker
docker-compose up
# use -d flag to run in background

# Tear down
docker-compose down

# To be able to edit files, add volume to compose file
volumes: ['./:/usr/src/app']

# To re-build
docker-compose build

#Insert Telegram token
1. Create a bot by talking to BotFather
2. Get Token API 
3. Visit https://api.telegram.org/bot<TokenID>/getUpdates. Get unique chat id
4. Paste <TELEGRAM_TO> and <TELEGRAM_TOKEN> into secrets under settings 
  (For example, the TELEGRAM_TO would only consists of numbers (0000000001) & TELEGRAM_TOKEN follows the ##########:xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx format.)

#Setting up the workflow
see workflow/telegram.yml
```

## Outcome
```bash
# Node/MongoDB app running in the same container
# Get Updates on telegram bot @Github_jinweiang_bot
```
