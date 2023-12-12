---
title: The Infraction System
weight: -10
---

Sangou's userlog system is very complex, but easy to understand.

<!--more-->

{{< toc >}}

## An overview

You can view a user's logs with the following command.

- `logs` [target]<br>
Displays logs for a user.

Logs will display all tosses, warns, kicks, bans, as well as the amount of notes they have.

With the exception of warns and notes, you do not have to add these logs yourself. Sangou will track tosses, kicks, and bans for you.

## Managing warnings

- `warn` [target] {reason}<br>
Warns a user. This will DM the user with the reason for their warning.

- `clearwarns` [target]<br>
This will clear all warnings for a user.

- `delwarn` [target] [index]<br>
This deletes a warning from a given index.

## Managing notes

Notes do not appear in the logs normally, to prevent cases where a user could see it themselves. Use the following commands for notes.

- `note` [target] {note}<br>
Adds a note to a user.

- `notes` [target]<br>
Shows the notes a target has.