---
title: Server Configuration
weight: -20
---

To get the most out of Dishwasher, you'll have to configure it for your server. The stock configuration (which you will see when downloading the configuration file for the first time) includes comments to assist you.

<!--more-->

{{< toc >}}

## Configuration commands

- `configs`<br>
Gives you the entire configuration file for the server.

![Example of Configs](/img/examples/configs-example.png)

- `configs set` [attachment of configuration file]<br>
Sets the configuration for the server.

- `configs reset` <br>
Resets the server's configuration.

- `configs stock` <br>
Shows the stock configuration.

## Configuration variables

This is a list of every configuration variable available in Dishwasher.

### Logging

{{< expand "Logging Settings" >}}
{{< propertylist name=config-logging >}}
{{< /expand >}}

### Staff

{{< expand "Staff Settings" >}}
{{< propertylist name=config-staff >}}
{{< /expand >}}

### Toss

{{< expand "Toss Settings" >}}
{{< propertylist name=config-toss >}}
{{< /expand >}}

### Surveyr

{{< expand "Surveyr Settings" >}}
{{< propertylist name=config-surveyr >}}
{{< /expand >}}

### CoTD

{{< expand "CoTD Settings" >}}
{{< propertylist name=config-cotd >}}
{{< /expand >}}

### Reaction

{{< expand "Reaction Settings" >}}
{{< propertylist name=config-reaction >}}
{{< /expand >}}

## Stock configuration

Below is the stock configuration, showing every available config setting, and its purpose. Do not edit the version variable.

```yaml
# These comments are here to get you started,
# and will go away upon setting the configuration
# for the first time. You can see these comments
# again by using the "configs stock" command.

# For any setting asking for an ID, you can put
# the name of it as well, and the bot will convert
# it to an ID automatically when you go to upload it.
# Note that it will use the first one it finds, and it is
# case-sensitive.
# For example:
# staffrole: "Server Staff"

logging:
  # The bot will forward moderation actions to this channel ID.
  modlog: 
  # The bot will forward server updates to this channel ID.
  serverlog: 
  # The bot will forward user updates to this channel ID.
  userlog: 

staff:
  # The role ID for the Staff role.
  staffrole: 
  # The role ID for the Ex-Staff role, if you use one.
  exstaffrole: 
  # The role ID for bots. This will allow bots to speak during lockdowns, and in toss channels.
  botrole: 
  # The role ID for new users, if Raidmode is set to Medium.
  raidrole: 
  # The role ID for the Staff channel.
  staffchannel: 
  # The channel ID which the bot will forward watched users to.
  watchchannel: 
  # A link to your rules. You can use channels with "<#CHANNELID>",
  # but the bot will not convert a name for you.
  rulesurl: 
  # A link to appeal bans or actions. This will be forwarded to
  # the user upon being banned by the bot.
  appealurl: 
  # If you would like Staff to be notified when a user continuously reply pings someone,
  # set this to the number of times after which the bot will notify Staff. Maximum of 10.
  noreplythreshold: 

toss:
  # The role ID to add to users when performing a toss.
  tossrole: 
  # The category ID for toss sessions to be created in.
  tosscategory: 
  # The channel names that the bot will use when creating sessions.
  # You may only have up to 25.
  tosschannels:
    - 
  # Optional, only if you wish for archival. Please ask the bot owner before configuring this.
  drivefolder: 

surveyr:
  # The channel ID that the bot will post moderation actions to.
  surveychannel: 
  # The case ID to start from, in the event that you are transitioning from a
  # previous system. If you aren't, simply leave it at 0, or 1 if you do not need a test case.
  startingcase: 
  # Pick from "ban", "unban", "kick", "softban", "timeout", "promotion", "demotion".
  loggingtypes:
    - 
  # If using "promotion" or "demotion" in Logging Types, place the role IDs you wish to monitor here.
  loggingroles:
    - 

cotd:
  # The role ID to use for a Color of The Day system.
  cotdrole: 
  # The name of the role. For example, "The Rainbow - Pale Blue", where "The Rainbow" is the role name.
  cotdname: 

reaction:
  # If the bot may pull message links and format them nicely.
  embedenable: false
  # If the bot may translate messages using reacted flags.
  translateenable: false
  # If the bot may autodelete super reactions.
  burstreactsenable: false
  # If the bot may automatically adjust names to be readable.
  autoreadableenable: false
  # If the bot may randomly laugh at users who have profile effects.
  # Some people get mad at this feature's existence for some reason.
  paidforprofileeffectsenable: false

metadata:
  version: 2
```
