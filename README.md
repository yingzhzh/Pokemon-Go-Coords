# Pokemon-Go-Coords
A web platform for crowdsourced Pokémon Go rare spawns coordinate data with a back-end Discord bot that parses known channels.

This is the official repository and first version of the [PokéSpawns web platform](http://spawns.sebastienvercammen.be).

Due to PokéSpawns registering as a company, further development will continue in private and any future versions won't be released on GitHub.

## Requirements
### Prerequisites
* [Node.js](https://nodejs.org/en/)

## Installation & Configuration
Install both the front-end and the back-end Discord bot by entering each folder and running `$ npm install`.

### Front-end
Configure your back-end bot's domain and port in [frontend/assets/js/main.js](frontend/assets/js/main.js).

Once all files are built (`npm run build`), you need to upload the `/public/` folder to your preferred webhost.

List of commands:

    npm run build       - Builds all required files
    npm run watch       - Watches all files for changes and builds them automatically on change

For technical people, there are more commands in [frontend/package.json](frontend/package.json), but these won't be required for installation only.

### Back-end Discord Bot
1. Rename [discord-bot/settings.json.example](discord-bot/settings.json.example) to `settings.json` and edit the settings.
2. Run the script with Node.js:
    `$ node index.js`