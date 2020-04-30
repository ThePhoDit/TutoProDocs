# Commands

This is a very important module. It will allow you to meticulously configure every command, individually.

 You will have the following configuration for every command:

```yaml
commands:
  ping:
    permission: 0
    enabled: true
    only_channels:
      - 'Channel ID 1'
      - 'Channel ID 2'
    disabled_channels:
      - 'Channel ID 1'
      - 'Channel ID 2'
  warn:
    permission: 50
    enabled: true
    only_channels: []
    disabled_channels: []
```

**Permission:** level needed to run the command. If the user has the same level or higher in the [levels module](levels.md), they will be able to run it. If you want to allow every user to use the command, set it to level `0`. By default, the bot uses the level associated to the command. Please check the [commands levels](../../commands/commands-levels.md) section.

**Enabled:** it can be `true` or `false`. If it is false, nobody can use the command. By default, true is used.

**Only Channels:** list of channels where the bot will only work. This overrides `disabled_channels`.

**Disabled Channels:** list of channels where the command cannot be used. By default, none of them are in there.

### Analyzing the Previous Example

So, in the previous example, we are going to see how would the warn command behave.

* Only users with level 50 or higher can use it.
* Everyone with the right permissions can run it, as it is enabled.
* It can be used in every channel, since the list is empty.

{% hint style="warning" %}
Remember that if a command is not there, the default configuration will be used.
{% endhint %}

