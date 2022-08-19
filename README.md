# TheDoctor

TheDoctor is in it's third iteration, now using DiscordJS v14 and build with slash commands.
This bot is hosted by me myself, but available to anyone that wants to use it's features.

[Click here to invite me to your server](https://discord.com/oauth2/authorize?client_id=1010203035261210724&permissions=277293903062&scope=applications.commands%20bot)
If you found any issues with the bot, please let me know by opening a [bug report](https://github.com/Master-Guy/TheDoctor/issues/new?labels=bug). Need more [documentation](https://github.com/Master-Guy/TheDoctor/issues/new?labels=documentation)? Or got a [suggestion](https://github.com/Master-Guy/TheDoctor/issues/new?labels=enhancement)? Please don't hesitate to ask and let me know!

## Current features

At this moment the bot already has the following functionalities available to use:

- [TheDoctor](#thedoctor)
  - [Current features](#current-features)
    - [Mass-assigning or revoking roles](#mass-assigning-or-revoking-roles)
    - [Sending DMs to users by the bot](#sending-dms-to-users-by-the-bot)
    - [Adding a number of messages to a channel](#adding-a-number-of-messages-to-a-channel)
    - [Removing a number of messages from a channel](#removing-a-number-of-messages-from-a-channel)
    - [Removing a number of messages by a specific user](#removing-a-number-of-messages-by-a-specific-user)
    - [Ping/Test to see if the bot is working properly](#pingtest-to-see-if-the-bot-is-working-properly)
  - [Planned and requested features](#planned-and-requested-features)

<br /><hr /><br />

### Mass-assigning or revoking roles

| Command                                        | Privilege required | Parameters                                                                                                                                              |
| ---------------------------------------------- | ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `/roles mass assign`<br />`/roles mass revoke` | `Manage Roles`     | 1: The `@role` to be assigned or revoked<br />2: `True` or `False` to indicate if the bot should only<br /> go through the users in the current channel |

`/roles mass assign @visitors False`<br />Will assign the `@visitors` role to all users in the server.

`/roles mass revoke @gamenight True`<br />Revoke the `@gamenight` role from all the users in the current channel.

<br /><hr /><br />

### Sending DMs to users by the bot

| Command   | Privilege required | Parameters                                                                                                                                          |
| --------- | ------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| `/senddm` | `Manage Messages`  | 1: The `@user` to send the message to<br />2: The `color` of the embed showing the message<br />3: The `message` actual message to show to the user |

`/senddm @randomuser Blue Thank you for helping us today!`<br />Will send a message to `@randomuser` showing as followed:<br />
![Example senddm](https://github.com/Master-Guy/TheDoctor/raw/main/senddm_example.png)

<br /><hr /><br />

### Adding a number of messages to a channel

| Command         | Privilege required | Parameters                                                 |
| --------------- | ------------------ | ---------------------------------------------------------- |
| `/messages add` | `Manage Messages`  | 1: The `amount` of messages to send to the current channel |

`/messages add 5`<br />Will send 5 messages to the current channel.
![Example messages add 5](https://github.com/Master-Guy/TheDoctor/raw/main/messagesadd_example.png)

<br /><hr /><br />

### Removing a number of messages from a channel

| Command            | Privilege required | Parameters                                                     |
| ------------------ | ------------------ | -------------------------------------------------------------- |
| `/messages remove` | `Manage Messages`  | 1: The `amount` of messages to remove from the current channel |

`/messages remove 5`<br />Will remove 5 messages from the current channel, starting with the latest.

<br /><hr /><br />

### Removing a number of messages by a specific user

| Command               | Privilege required | Parameters                                                                                                                                                    |
| --------------------- | ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `/messages remove_by` | `Manage Messages`  | 1: The `@user` who's messages to remove<br />2: The `amount` of messages to remove <br />3: `True` or `False` indicating to remove messages from all channels |

`/messages remove_by @naughtyuser 5 False`<br />Will remove the last 5 messages made by `@naughtyuser` in the current channel.

`/messages remove_by @banneduser 5 True`<br />Will remove the last 5 messages made by `@banneduser` in each channel of this server.

<br /><hr /><br />

### Ping/Test to see if the bot is working properly

| Command              | Privilege required       | Parameters   |
| -------------------- | ------------------------ | ------------ |
| `/ping`<br />`/test` | N/A<br />`Administrator` | N/A<br />N/A |

`/ping`<br />
Will have the bot respond with `Pong!`

`/test`<br />
Will have the bot respond with `Test OK!`

<br /><hr /><br />

## Planned and requested features

Currently planned features are listed here, but feel free to suggest more.

-   GitHub.com repository messages to report new or updated Pull Requests, Issues and Releases
