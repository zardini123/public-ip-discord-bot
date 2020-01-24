# Public IP Discord Bot

A Discord Bot that displays the public ip of the server running it. This implementation has the bot manage a single text channel. If any user types in the selected channel, the bot will clear all message and post the current ip. The public ip will be checked in the background every `INTERVAL`, as defined in the environment variables.

## Configuration

Configuration is done through a _.env_ file located in the root of this project. The following environment variables are used:

`TOKEN`: The Token of the Bot, provided by Discord (**not** the application Client ID or the Client Secret)

`CHANNEL`: The id for the text channel used for the bot. Setting a Discord client to Developer Mode can be used to find this id.

`INTERVAL`: The interval (in milliseconds) the bot will check if the ip has changed. Example: `INTERVAL=2000` will check every 2 seconds.
