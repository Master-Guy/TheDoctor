# TheDoctor

TheDoctor is in it's third iteration, now using DiscordJS v14 and build with slash commands.
This bot is hosted by me myself, but available to anyone that wants to use it's features.

## Current features

At this moment the bot already has the following functionalities available to use:

-   Mass-assigning or revoking roles
-   Sending DMs to users by the bot
-   Adding a number of messages to a channel
-   Removing a number of messages from a channel
-   Removing a number of messages by a specific user
-   Ping/Test to see if the bot is working properly

### Mass-assigning or revoking roles

| Command                                        | Privilege required | Description                                         | Parameters                                                                                                                                              | Example                                                                                                                                                                                                                     |
| ---------------------------------------------- | ------------------ | --------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `/roles mass assign`<br />`/roles mass revoke` | `Manage Roles`     | Mass-assigns or mass-revokes roles to or from users | 1: The `@role` to be assigned or revoked<br />2: `True` or `False` to indicate if the bot should only<br /> go through the users in the current channel | `/roles mass assign @visitors False`<br />Will assign the `@visitors` role to all users in the server<hr />`/roles mass revoke @gamenight True`<br />Revoke the `@gamenight` role from all the users in the current channel |

-   Roles
    -   Command: `/roles mass assign` or `/roles mass revoke`
    -   Parameter 1: The `@role` to be assigned or revoked
    -   Parameter 2: `True` if the bot should only go through the users in the current channel, or `False` if the bot should go through all users in the server
    -   Privilege required: `Manage Roles`
-   Sending DMs to users by the bot
    -   Command: `/senddm`
    -   Parameter 1: The `@user` to send the message to
    -   Parameter 2: The `color` of the embed showing the message
    -   Parameter 3: The `message` actual message to show to the user
    -   Privilege required: `Manage Messages`
-   Adding a number of messages to a channel
    -   Command: `/messages add`
    -   Parameter 1: The `amount` of messages to send to the current channel
    -   Privilege required: `Manage Messages`
-   Removing a number of messages from a channel
    -   Command: /messages remove
    -   Requires the `Manage Messages` privilege
-   Removing a number of messages by a specific user from either a single channel, or from all channels in the server
    -   Command: /messages remove_by
    -   Requires the `Manage Messages` privilege
-   And of course Ping/Test to see if the bot is working properly
    -   Commands: /ping and /test
    -   Available for everyone, without permissions

## Future features

Currently planned features are listed here, but feel free to suggest more.

-   GitHub.com repository messages
    -   Command: /github
    -   Requires the `Manage webhooks` privilege
