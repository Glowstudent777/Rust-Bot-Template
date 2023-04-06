# Rust Bot Template

This repo contains the code that runs the [Gitpod Community Discord Bot](https://github.com/gitpod-io/optimus). I'm attempting to strip it down to make it the perfect template.

Community contribuitions are welcome! 🧡

# Contributing

You wanna contribute!? That sounds awesome! Thank you for taking the step to contribute towards this project :)

## Getting started

> Creating the Bot application on Discord's dev portal
- Login on https://discord.com/developers/applications
- Create a new app by clicking on `New Application` on the top right
- Inside your bot page, click on 🧩 `Bot` from the left sidebar and then `Add Bot` button
    - In the same page, toggle on the following options: `Presence Intent`, `Server Members Intent` and `Message Content Intent`
- Go to **OAuth2 > URL Generator** from your left sidebar
    - Tick `Scopes: bot, application.commands` and `Bot permissions: Adminstrator`. It should look like below:
    ![OAuth2 example](/.assets/oauth2_example.png)
    - Scroll to the bottom of this page and copy paste the **GENERATED-URL** into your browser tab to add the bot to a discord server. I recommend creating a new Discord server for bot development perposes.

> Running the Bot

- Grab the token from your 🧩 `Bot` page on discord dev portal. You might need to reset it to see.
![bot token](/.assets/bot_token_example.png)
- Grab the **Application ID** from the `General Information` section in your left sidebar
- Rename `.env.example` to `.env` and fill in the values
```env
DISCORD_TOKEN=
APPLICATION_ID=
```
- Run the bot by using this command in the terminal
```bash
cargo run
```
