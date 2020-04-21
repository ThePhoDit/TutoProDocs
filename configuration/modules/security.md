---
description: This is a premium module.
---

# Security

This module allows you to secure your server. This can be used as a server gatekeeper but you can do with it anything your imagination can come up with.

The configuration is super simple:

```yaml
security:
  ignored_users: []
  access:
    - password: 'Password 1'
      roles:
        - 'Role ID 1'
        - 'Role ID 2'
    - password: 'Password 2'
      roles:
        - 'Role ID 3'
```

**Ignored Users:** list of users that can't use this module.

**Access:** list of passwords and roles. You can add as many as you want. This is the structure:

* **Password:** the secret code users have to introduce using the password command.
* **Roles:** list of roles that will be added if the user has the right code. 

