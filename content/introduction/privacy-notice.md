---
title: Privacy Notice
weight: -10
---

By default, Sangou will collect analytics about how he is being used.

<!--more-->

{{< toc >}}

## As a User

Your analytics are stored in `data/users/{user ID}/analytics.json`.

Analytics stored currently include:
- Successful command
- Failed command

More may be added at a later time.

Manage your analytics with the following commands:

- `mydata`<br>
This will give you all of the data the bot has for you in its `users/YOURID` folder.<br>
This does not include reminders.

- `stats`<br>
Shows a prettified version of your analytics file.

- `stats disable`<br>
Disables analytics collection for you and delete all analytics data currently saved.

- `stats enable`<br>
Enables analytics collection for you if it was previously disabled.

## As a Server

Your server's analytics are stored in `data/servers/{server ID}/analytics.json`.

Server analytics are not currently implemented.
