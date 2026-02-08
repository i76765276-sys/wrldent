# Workspace

Workspace is a lightweight, prefix-based Discord bot framework built on top of discord.js.

## Installation

    npm install workspace discord.js dotenv

## Quick Start

    require('dotenv').config();
    const BotClient = require('workspace');

    const bot = new BotClient({
      prefix: '!',
      commandsPath: './commands',
      eventsPath: './events'
    });

    bot.start(process.env.TOKEN);

## Project Structure

    your-bot/
    ├── index.js
    ├── .env
    ├── commands/
    │   └── ping.js
    ├── events/
    │   └── ready.js
    └── package.json

## BotClient API

Constructor options:
- prefix (string)
- commandsPath (string)
- eventsPath (string)

Methods:
- start(token)
- loadCommands()
- loadEvents()
- listenForCommands()

## License

MIT
