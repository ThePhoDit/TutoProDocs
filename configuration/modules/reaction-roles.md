# Reaction Roles

Make users select which roles they want to have.

```yaml
reaction_roles:
  - message: 'Message ID'
    emoji: '👺' # For default emojis.
    roles:
      - id: 'Role ID 1'
        type: 'ADD'
      - id: 'Role ID 2'
        type: 'REMOVE'
  - message: 'Message ID'
    emoji: 'tester:714804405806956685' # For custom emojis (name:id)
    roles:
      - id: 'Role ID 3'
```

Reaction Roles configuration is a list with different objects as you want. Every object corresponds to a message and an emoji:

**Message:** the ID of the message where the reaction role will be.

**Emoji:** the emoji that users have to react to. Paste the Unicode emoji if it is a default one or use the format _name:id_ for custom ones.

**Roles:** list of roles to add or remove on react:

* **ID:** the role ID.
* **Type:** `ADD` or `REMOVE`. Defaults to ADD.

{% hint style="info" %}
Remember that you have to manually add the reaction to the message.
{% endhint %}



