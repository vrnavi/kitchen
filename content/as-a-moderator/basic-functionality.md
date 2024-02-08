---
title: Basic Functionality
weight: -20
---

Like any Discord bot, Sangou has tools at your disposal to moderate users.

<!--more-->

{{< toc >}}

{{< hint type=note title="Please note!" >}}
For your reference:
- **[argument]** represents a required argument.
- **{argument}** is an optional requirement.
- argument **(default)** is the default if not specified.

Sangou uses the `pls` invoker by default.

For example: `pls command [required (default)] {optional (default)}`
{{< /hint >}}

## Banning

- `ban` [target] {reason}<br>
Bans a user and messages them with the reason.

- `dban` [target] [duration] {reason}<br>
Bans a user with a specified amount of days worth of messages deleted, messages them with the reason.

- `massban` [targets]<br>
Bans several users with their IDs without messaging them.

- `sban` [target] {reason}<br>
Bans a user without messaging them. You can also use the traditional ban method to achieve the same effect.

- `unban` [target] {reason}<br>
Unbans a user.

### Kicking

- `kick` [target] {reason}<br>
Kicks a user.

## Lockdown

- `lock` {channel (current)} {soft (false)}<br>
Prevents people from speaking. Will have a "hard" tone by default.<br>
Use true/false with the "soft" argument to adjust this behavior.

- `unlock` {channel (current)}<br>
Unlocks the current channel for speaking.

## Purging

- `purge` {limit (50)} {channel (current)}<br>
Clears a given number of messages.

- `purge bots` {limit (50)} {channel (current)}<br>
Clears a given number of bot messages.

- `purge from` [user] {limit (50)} {channel (current)}<br>
Clears a given number of messages from a user.

- `purge with` [string] {limit (50)} {channel (current)}<br>
Clears a given number of messages with a certain string.

- `purge emotes` {limit (50)} {channel (current)}<br>
Clears a given number of messages with emotes.

- `purge embeds` {limit (50)} {channel (current)}<br>
Clears a given number of messages with embeds, including stickers.

- `purge reacts` {limit (50)} {channel (current)}<br>
Clears a given number of reactions from messages.<br>
This will not delete the messages themselves.

## Miscellaneous

- `alert` [target]<br>
Awaits a member's next message for up to a day.

- `nickname` [target] {nickname}<br>
Sets a users nickname. Send command by itself to reset.

- `reroll`<br>
Forcibly rerolls the current Color of The Day.
