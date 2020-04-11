# Logs

This module allows you to log everything that happens in your server. As always, let's see an example first:

```yaml
logs:
  timezone: 'Europe/Madrid'
  ignored_roles: []
  ignored_channels: []
  ignored_users: []
  channels:
    - id: 'Channel ID'
      enabled: true
      include:
        - 'WARN'
        - 'KICK'
        - 'BAN_ADD'
        - 'TEMPBAN_ADD'
        - 'BAN_RMV'
        - 'MUTE_ADD'
        - 'MUTE_RMV'
        - 'TEMPMUTE_ADD'
        - 'GUILD_MEMBER_ADD'
        - 'GUILD_MEMBER_RMV'
        - 'VOICE_JOIN'
        - 'VOICE_MOVE'
        - 'VOICE_LEAVE'
        - 'MESSAGE_EDIT'
        - 'MESSAGE_DELETE'
        - 'CENSOR'
        - 'COMMAND_USED'
        - 'SPAM'
        - 'CHANNEL_CREATE'
        - 'CHANNEL_UPDATE'
        - 'CHANNEL_DELETE'
```

**Timezone:** region that the bot will use to get the date. You can see all available timezones [here](https://timezonedb.com/time-zones) \(please check the Time Zone column\).

**Ignored Roles:** list of roles IDs that are not logged. If a user has one of those roles, they're invisible to the logs.

**Ignored Channels:** list of channels IDs that won't appear on the logs.

**Ignored Users:** list of users IDs that will not have any action registered.

**Channels:** remember, you can add as many as you want.

* **ID:** ID of the channel where logs will be sent.
* **Enabled:** whether if the logs for that channel are enabled or not. It can be `true` or `false`. Default is  false.
* **Include:** list of actions that are sent into that channel. Names are really descriptive, so just read them.



