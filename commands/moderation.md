---
description: >-
  Here you will find all the moderation commands that you can use with TutoPro.
  If a command has an alias, all of the ways of using it will be shown.
---

# Moderation

### Search for a specific user infractions:

```text
;infractions {user}
---------
;infrs {user}
```

### Change the reason of an infraction:

```text
;reason {infraction ID} {new reason}
```

### Change the duration of an infraction:

```text
;duration {infraction ID} {new duration}
```

> Only works on temporary infractions.

### Warn someone:

```text
;warn {user} [reason]
```

### Mute someone:

```text
;mute {user} [reason]
```

> Mute Role is required in the [Infractions module](../configuration/modules/infractions.md).

### Temporarily mute someone:

```text
;tempmute {user} {duration} [reason]
```

> Mute Role is required in the [Infractions module](../configuration/modules/infractions.md).

### Unmute a muted user:

```text
;unmute {user} [reason]
```

> Mute Role is required in the [Infractions module](../configuration/modules/infractions.md).

### Kick someone from the server:

```text
;kick {user} [reason]
```

### Ban someone:

```text
;ban {user} [reason]
```

### Temporarily ban someone:

```text
;tempban {user} {duration} [reason]
```

### Unban someone who is banned:

```text
;unban {user} [reason]
```

{% hint style="info" %}
#### Showing the Moderator

Infractions notifications will show the moderator when notifying an user based on the [Infractions configuration](../configuration/modules/infractions.md).

This can be overridden by introducing a keyword between the user/duration and the reason when running the command. The available keywords are:

**DM** - It will always show who gave the infraction.

Example: `;warn {user} DM [reason]`

**ADM** - It will never show who gave the infraction

Example: `;warn {user} ADM [reason]`
{% endhint %}

