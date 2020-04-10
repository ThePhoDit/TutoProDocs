# Joins

You can set custom messages that are sent when a new user joins your server.

```yaml
joins:
  enabled: true
  channels:
    - id: 'Channel ID 1'
      message: |-
        Hello {{member}}, welcome to {{server}}
    - id: 'Channel ID 2'
      message: |-
        Hello {{member}}, welcome to my Server.
```

**Enabled:** whether this module is enabled or not.

**Channels:** this is a list of channels and messages. Each item if formed by:

* **ID:** The ID of the channel where the message is sent.
* **Message:** the actual message. There are some variables that you can use here:
  * **{{member}}** - Mentions the new user.
  * **{{memberTag}}** - Replaces it for the user tag, such as TutoPro\#4702.
  * **{{memberCount}}** - Displays the amount of members in your server.

{% hint style="info" %}
You can add as many channels as you like.
{% endhint %}

