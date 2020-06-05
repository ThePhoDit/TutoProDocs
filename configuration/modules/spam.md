# Spam

Spam module keeps away to users who try to flood the chat spamming messages. You can filter by an amount of messages, an amount of duplicated messages or by the number of lines in a message.

Here you have an example of how it is configured:

```yaml
spam:
  enabled: true
  level_whitelist: 40
  delete_messages: true
  tempmute_duration: 900
  channels_whitelist: []
  roles_whitelist: []
  users_whitelist: []
  maximum_messages:
    enabled: true
    amount: 10
    interval: 5
    channels_whitelist: []
    roles_whitelist: []
    users_whitelist: []
  duplicated_messages:
    enabled: true
    amount: 5
    interval: 5
    channels_whitelist: []
    roles_whitelist: []
    users_whitelist: []
  maximum_lines:
    enabled: true
    amount: 5
    channels_whitelist: []
    roles_whitelist: []
    users_whitelist: []
```

**Enabled:** whether this module is on or off.

**Level Whitelist:** level that someone needs to be ignored. Anyone with higher level won't trigger the filter.

**Delete Messages:** whether the bot deletes the messages or not.

**Tempmute Duration:** time in seconds of the applied mute. Set it to 0 to disable it.

**Roles Whitelist:** list of roles globally ignored.

**Channels Whitelist:** list of channels globally ignored.

**Users Whitelist:** list of users globally ignored.

{% tabs %}
{% tab title="Maximum Messages" %}
**Enabled:** whether this section is enabled or disabled.

**Amount:** amount of messages that trigger the filter.

**Interval:** time in seconds to send the selected amount of messages.

**Roles Whitelist:** list of ignored roles.

**Channels Whitelist:** list of ignored channels.

**Users Whitelist:** list of ignored users.
{% endtab %}

{% tab title="Duplicated Messages" %}
**Enabled:** whether this section is enabled or disabled.

**Amount:** amount of duplicated messages that trigger the filter.

**Interval:** time in seconds to send the selected amount of duplicated messages.

**Roles Whitelist:** list of ignored roles.

**Channels Whitelist:** list of ignored channels.

**Users Whitelist:** list of ignored users.
{% endtab %}

{% tab title="Maximum Lines" %}
**Enabled:** whether this section is enabled or disabled.

**Amount:** amount of lines in a message that trigger the filter.

**Roles Whitelist:** list of ignored roles.

**Channels Whitelist:** list of ignored channels.

**Users Whitelist:** list of ignored users.
{% endtab %}
{% endtabs %}

