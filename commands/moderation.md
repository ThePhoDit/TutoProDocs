---
description: >-
  Here you will find all the moderation commands that you can use with TutoPro.
  If a command has an alias, all of the ways of using it will be shown.
---

# Moderation

### Search for a specific user infractions: \(60\)

```text
;infractions {user}
---------
;infrs {user}
```

### Change the reason of an infraction: \(60\)

```text
;reason {infraction ID} {new reason}
```

### Change the duration of an infraction: \(60\)

```text
;duration {infraction ID} {new duration}
```

### Delete an infraction: \(60\)

```text
;delete {infraction ID}
```

> Only works on temporary infractions.

### Warn someone: \(60\)

```text
;warn {user} [reason]
```

### Mute someone: \(60\)

```text
;mute {user} [reason]
```

> Mute Role is required in the [Infractions module](../configuration/modules/infractions.md).

### Temporarily mute someone: \(60\)

```text
;tempmute {user} {duration} [reason]
```

> Mute Role is required in the [Infractions module](../configuration/modules/infractions.md).

### Unmute a muted user: \(60\)

```text
;unmute {user} [reason]
```

> Mute Role is required in the [Infractions module](../configuration/modules/infractions.md).

### Kick someone from the server: \(60\)

```text
;kick {user} [reason]
```

### Ban someone: \(60\)

```text
;ban {user} [reason]
```

### Temporarily ban someone: \(60\)

```text
;tempban {user} {duration} [reason]
```

### Unban someone who is banned: \(60\)

```text
;unban {user} [reason]
```

### Clean messages: \(60\)

```text
;clean {amount}
or
;clean {user} {amount}
```

### Ban multiple users: \(60\)

```text
;mban {users} [-r] [reason]
```

> User IDs must be separated by a space. The -r tag means that the reason starts from there.

### Kick someone from a voice channel: \(60\)

```text
;voicekick {user}
```

### Get the list of server roles: \(60\)

```text
;roles
```

### Change the slowmode time of the curresnt channel: \(40\)

```text
;slowmode {time in seconds}
```

### Lock a channel: \(60\)

```text
;lock [roles]
```

> Roles must be separated by spaces. If none, everyone is used.

### Unlock a channel: \(60\)

```text
;unlock [roles]
```

> Roles must be separated by spaces. If none, everyone is used.

{% hint style="info" %}
#### Showing the Moderator

Infractions notifications will show the moderator when notifying an user based on the [Infractions configuration](../configuration/modules/infractions.md).

This can be overridden by introducing a keyword between the user/duration and the reason when running the command. The available keywords are:

**DM** - It will always show who gave the infraction.

Example: `;warn {user} DM [reason]`

**ADM** - It will never show who gave the infraction

Example: `;warn {user} ADM [reason]`
{% endhint %}



