# Selfhosting the 2b2t.jp bot

## Requirements
- [Node.js](https://nodejs.org/)

## Optional
- [yarn](https://yarnpkg.com/) (optional, but recommended. you can install via `npm i -g yarn`)

## Run the bot

### Quick start
- Clone https://github.com/acrylic-style/2b2t.jp-bot
- Modify `.env`
  - `prefix` - prefix, you can run commands with `<prefix><command>`
  - `token` - the bot token ([discord developer portal](https://discord.com/developers/applications/))
  - `endPoint` - data.json URL (to fetch server status), example: `https://status.2b2t.jp/api/data.json`
  - `seed` - server seed (will be shown in `!seed`)
- Run `npm install` or `yarn`
- Start the application using `node index.js` or similar things
