# Censor

Censor plugin allows you to control if users can self-advertise or send blacklisted words. We will be going through all the properties after seeing and example, as usual:

When something triggers this module, the message is deleted and sent to the logs channel with the `CENSOR` tag in the include section.

```yaml
censor:
  level_whitelist: 40
  
  filter_invites: true
  invites_codes_whitelist:
    - 'minecraft'
    - 'aUNhdFD'
  invites_guilds_whitelist:
    - 'Guild ID 1'
  invites_channels_whitelist: []

  filter_links: true
  links_domains_whitelist:
    - 'google.com'
    - 'twitch.tv'
  links_channels_whitelist:
    - 'Channel ID 1'
    - 'Channel ID 2'

  filter_tokens: true
  tokens_blacklist:
    - 'Token 1'
    - 'Token 2'
  tokens_channels_whitelist:
    - 'Channel ID 1'
    - 'Channel ID 2'
    - 'Channel ID 3'

  filter_words: true
  words_blacklist:
    - 'Word 1'
    - 'Word 2'
  words_channels_whitelist: []
```

  
**Level Whitelist:** here you set the level the module will affect to. If the user has [level](levels.md) 50 and censor is set to 40, the user won't activate the filter. It will only be triggered if the user has the same level or lower.

{% tabs %}
{% tab title="Invites" %}
**Filter Invites:** Whether Discord servers invites should be censored or not. It can be `true` or `false`.

**Invites Codes Whitelist:** list of specific invites that won't be deleted. Make sure you just put the invite code.

**Invites Guilds Whitelist:** list of servers which invites won't be deleted, this means that, if an X server is there, none of the invites belonging to it will be censored.

**Invites Channels Whitelist:** list of channels where this section of the module will be disabled. Any invite will be allowed.
{% endtab %}

{% tab title="Links" %}
**Filter Links:** Whether URLs that are not invites should be censored or not. It can be `true` or `false`.

**Links Domains Whitelist:** list of domains that will be ignored by TutoPro.

**Links Channels Whitelist:** list of channels where this section of the module will be disabled. Any URL will be allowed.
{% endtab %}

{% tab title="Words" %}
**Filter Words:** Whether blacklisted words should be censored or not. It can be `true` or `false`.

**Words Blacklist:** list of words that will be censored by the bot.

**Words Channels Whitelist:** list of channels where this section of the module will be disabled.
{% endtab %}

{% tab title="Tokens" %}
**Filter Tokens:** Whether blacklisted tokens should be censored or not. It can be `true` or `false`.

**Tokens Blacklist:** list of tokens that will be deleted.

**Tokens Channels Whitelist:** list of channels where this section of the module will be disabled. Any token will be accepted.
{% endtab %}
{% endtabs %}

{% hint style="info" %}
### What is the difference between words and tokens?

If it's your first time using one bot of this type, we understand your confusion.

#### Words

Words are always **separated by one space** on each side. If `Hello` was a blacklisted word:

Hello I'm PhoDit -&gt; Would be deleted.

Hello, I'm PhoDit -&gt; Wouldn't be deleted.

#### Tokens

Tokens can be anywhere inside a message. If `Hello` was a blacklisted token:

Hello I'm PhoDit -&gt; Would be deleted.

Hello, I'm PhoDit -&gt; Would be deleted.

I like sayingthetoken**Hello**lol -&gt; Would be deleted.
{% endhint %}

{% hint style="warning" %}
Remember that words and tokens are case insensitive.
{% endhint %}

