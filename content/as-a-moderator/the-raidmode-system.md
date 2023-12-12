---
title: The Raidmode System
weight: 30
---

The Raidmode system has a few options to get a handle on a raid, aside from using Discord's standard fare.

Raidmode requires a `staffchannel` to be configured. The Medium option requires a `raidrole` to be configured.

<!--more-->

{{< toc >}}

## Configuration

- `raidmode`<br>
Opens the Raidmode configuration screen.

![Raidmode Configuration](/img/examples/raidmode-example.png)

### Off

When set to Off, Sangou will only forward users under 24 hours old to the Staff channel.

### Low

When set to Low, Sangou will forward all new users to the Staff channel.

![Raidmode Low Example](/img/examples/raidmode-low-example.png)

### Medium

Medium can only be selected if `raidrole` is configured.

An example use case for Medium would be to filter new users during a raid.

### High

This is self explanatory. All new users will be kicked from the server.

## Message awaiting

In all cases where Sangou forwards a new user to the Staff channel, it will wait for their first proper message.

This is very useful in the event that you need to quickly see if a new user is spamming scam messages.

![Raidmode Message Example](/img/examples/raidmode-message-example.png)

