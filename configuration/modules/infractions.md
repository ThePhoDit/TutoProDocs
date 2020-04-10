# Infractions

Here you will configure the moderation part of the bot. We are going to see an example first and I will show you what everything is for afterwards.

```yaml
infractions:
  mute_role: 'Mute Role ID'
  notify:
    - 'WARN'
    - 'MUTE'
    - 'TEMPMUTE'
    - 'UNMUTE'
    - 'KICK'
    - 'BAN'
    - 'TEMPBAN'
    - 'UNBAN'
  show_moderator: false
```

**Mute Role:** this is the role that is given to users when they are muted by a moderator or by the spam filter.

**Notify:** all the actions of this list will be notified to a user when they are punished. If you don't want them to receive any notification, just remove the action from here.

**Show Moderator:** whether to show the moderator who gave the infraction to the notified user or not. You will see that this can be overridden when using a command in the moderation commands section.

