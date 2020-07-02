# Leaves

Leaves module works exactly in the same way as the joins one, but it is activated when someone leaves the server.

```yaml
leaves:
  enabled: true
  channels:
    - id: 'Channel ID 1'
      message: |-
        See you {{member}}, welcome to {{server}}
```

**Enabled:** whether this module is enabled or not.

**Channels:** this is a list of channels and messages. Each item if formed by:

* **ID:** The ID of the channel where the message is sent.
* **Message:** the actual message. There are some variables that you can use here:
  * **{{member}}** - Mentions the new user.
  * **{{memberTag}}** - Replaces it for the user tag, such as TutoPro\#4702.
  * **{{memberCount}}** - Displays the amount of members in your server.
  * **{{server}}** - Server's name.
* **Embed:** whether if an embed should be used or not.
* **Random:** list of messages from where TutoPro will choose a random one.

