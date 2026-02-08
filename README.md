# Workspace

Workspace is a lightweight, prefix-based Discord bot framework built on top of discord.js.

## Installation

    npm install workspace discord.js dotenv

## Quick Start

    require('dotenv').config();
    const Workspace = require('workspace');

    const bot = new Workspace({
      prefix: '!',
      commandsPath: './commands',
      eventsPath: './events'
    });

    bot.start(process.env.TOKEN);



## License

MIT
