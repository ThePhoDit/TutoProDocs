# Spam

This module prevents users from spamming multiple or duplicated messages. Let's see how it is configured:

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
    interval: 5
    channels_whitelist: []
    roles_whitelist: []
    users_whitelist: []
```

**Enabled:** whether this module is enbaled or not.

**Level Whitelist:** Users with a higher level in the levels module than the configured here won't activate the filter.

**Delete Messages:** whether messages are deleted or not after triggering the module.

**Tempmute Duration:** duration in seconds of the mute that is applied to the user. If set to 0, it doesn't mute.

**Channels Whitelist:** list of channels where this module is disabled.

**Roles Whitelist:** list of roles that will be ignored.

**Users Whitelist:** list of users that will be ignored.

{% tabs %}
{% tab title="Maximum Messages" %}
**Enabled:** whether this section is enabled  or not.

**Amount:** quantity of messages that activate the filter.

**Interval:** time in seconds in which the amount of messages should be sent.

**Channels Whitelist:** list of channels where this section is disabled.

**Roles Whitelist:** list of roles that will be ignored.

**Users Whitelist:** list of users that will be ignored.
{% endtab %}

{% tab title="Duplicated Messages" %}
**Enabled:** whether this section is enabled or not.

**Amount:** quantity of messages that activate the filter.

**Interval:** time in seconds in which the amount of messages should be sent.

**Channels Whitelist:** list of channels where this section is disabled.

**Roles Whitelist:** list of roles that will be ignored.

**Users Whitelist:** list of users that will be ignored.
{% endtab %}

{% tab title="Maximum Lines" %}
**Enabled:** whether this section is enabled or not.

**Amount:** quantity of lines that activate the filter.

**Interval:** time in seconds in which the amount of lines should be sent.

**Channels Whitelist:** list of channels where this section is disabled.

**Roles Whitelist:** list of roles that will be ignored.

**Users Whitelist:** list of users that will be ignored.
{% endtab %}
{% endtabs %}

